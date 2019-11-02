<template>
  <section class="home">
    <h1 class="title">
      KOHEI SUZUKI<br />
      PROFILE
    </h1>
    <h2 class="message">
      株式会社エスワイシステムのエンジニア、鈴木晃平の職務経歴サイトです。<br />
      少しでもわたしのことをお伝えできましたら幸いです。
    </h2>
    <a href="https://github.com/Kou0402" target="_blank" class="github">
      <img :src="githubIconPath" class="icon" />
    </a>
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
  padding: 90px 0;
  > .title {
    color: $main-color1;
    font-size: 6rem;
    margin-bottom: 20px;
  }
  > .message {
    color: $main-color1;
    font-size: 2rem;
    font-weight: 500;
    margin-bottom: 80px;
  }
  > .github {
    float: right;
    > .icon {
      width: 40px;
    }
  }
}
</style>
