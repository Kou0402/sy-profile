<template>
  <section class="home">
    <h1 class="title">
      KOHEI SUZUKI<br />
      PROFILE
    </h1>
    <h3 class="message">
      株式会社エスワイシステムのエンジニア、鈴木晃平の職務経歴サイトです。<br />
      少しでもわたしのことをお伝えできましたら幸いです。
    </h3>
    <div class="github">
      <p class="guide">ソースはこちら→</p>
      <a href="https://github.com/Kou0402" target="_blank">
        <img :src="githubIconPath" class="icon" />
      </a>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      githubIconPath: require('~/assets/image/' + 'github_icon.svg')
    }
  }
}
</script>

<style lang="scss" scoped>
.home {
  padding: 72px 0;
  > .title {
    margin-bottom: 28px;
    line-height: 7.2rem;
  }
  > .message {
    font-size: 2rem;
    font-weight: 500;
    line-height: 3.2rem;
    margin-bottom: 144px;
  }
  > .github {
    display: flex;
    font-size: 1.5rem;
    align-items: center;
    float: right;
    > .guide {
      margin-right: 4px;
    }
    .icon {
      width: 40px;
      animation: key1 0.4s ease infinite alternate;
    }
    @keyframes key1 {
      0% {
        transform: translateY(0px);
      }
      100% {
        transform: translateY(-10px);
      }
    }
  }
}
</style>
