<template>
  <div>
    <header class="header">
      <NavBar></NavBar>
    </header>
    <main class="main">
      <nuxt />
    </main>
  </div>
</template>

<script>
import NavBar from '~/components/layout/NavBar.vue'

export default {
  components: {
    NavBar
  }
}
</script>

<style lang="scss" scoped>
.header {
  margin: 70px 13vw 0 13vw;
}
.main {
  margin: 40px 13vw;
}
</style>
