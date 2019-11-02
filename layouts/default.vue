<template>
  <div>
    <header>
      <NavBar></NavBar>
    </header>
    <main>
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
