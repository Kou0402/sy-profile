<template>
  <section class="home">
    <div class="title">
      <transition appear name="name">
        <h1>KOHEI SUZUKI</h1>
      </transition>
      <transition appear name="profile">
        <h1>PROFILE</h1>
      </transition>
    </div>
    <h3 class="message">
      株式会社エスワイシステムのエンジニア鈴木晃平の職務経歴サイトです。<br />
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

    // transition
    > .name-enter-active {
      transition: all 1.2s ease 0s;
      -webkit-transition: all 1.2s ease 0s;
    }
    > .profile-enter-active {
      transition: all 1.2s ease 0.3s;
      -webkit-transition: all 1.2s ease 0.3s;
    }
    > .name-enter,
    > .profile-enter {
      opacity: 0;
      transform: translateY(30px);
      -webkit-transform: translateY(30px);
    }
    > .name-enter-to,
    > .profile-enter-to {
      transform: translateY(0);
      -webkit-transform: translateY(0);
    }
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

@media screen and (max-width: 560px) {
  .home {
    padding: 40px 0;
    > .title {
      margin-bottom: 16px;
      line-height: 6.4rem;
    }
    > .message {
      font-size: 1.6rem;
      margin-bottom: 80px;
      padding-right: 32px;
    }
  }
}
</style>
