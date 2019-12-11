<template>
  <nav class="nav-bar">
    <NavLink path="/">ホーム</NavLink>
    <NavLink path="about">自己紹介</NavLink>
    <NavLink path="carrier">職務経歴</NavLink>
    <NavLink path="skill">スキル</NavLink>
    <nuxt-link to="/" class="logo"
      ><img :src="navIconPath" class="image"
    /></nuxt-link>
  </nav>
</template>

<script>
import NavLink from '~/components/layout/NavLink.vue'

export default {
  components: {
    NavLink
  },
  data() {
    return {
      navIconPath: require('~/assets/image/' + 'nav_icon.png')
    }
  }
}
</script>

<style lang="scss" scoped>
.nav-bar {
  display: flex;
  height: 48px;
  align-items: center;
  border-bottom: solid 2px $main-color1;
  > .nav-link {
    margin-right: 32px;
  }
  > .logo {
    margin-left: auto;
    > .image {
      height: 44px;
      margin-bottom: 10px;
    }
  }
}

@media screen and (max-width: 560px) {
  .nav-bar {
    > .nav-link {
      margin-right: 8px;
    }
  }
}
</style>
