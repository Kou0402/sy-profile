<template>
  <nav class="nav-bar">
    <NavLink path="about">自己紹介</NavLink>
    <NavLink path="carrier">職務経歴</NavLink>
    <NavLink path="skill">スキル</NavLink>
    <nuxt-link to="/" class="logo">KS</nuxt-link>
  </nav>
</template>

<script>
import NavLink from '~/components/layout/NavLink.vue'

export default {
  components: {
    NavLink
  }
}
</script>

<style lang="scss" scoped>
.nav-bar {
  display: flex;
  background-color: $base-color;
  height: 60px;
  align-items: center;
  border-bottom: solid 2px $main-color1;
  > .nav-link {
    margin-right: 40px;
  }
  > .logo {
    color: $main-color1;
    font-size: 3rem;
    text-decoration: none;
    margin-left: auto;
    font-family: 'Architects Daughter', cursive;
  }
}
</style>
