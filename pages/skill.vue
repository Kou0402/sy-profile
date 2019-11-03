<template>
  <section class="skill">
    <FrontendArea></FrontendArea>
    <BackendArea></BackendArea>
    <ToolArea></ToolArea>
  </section>
</template>

<script>
import FrontendArea from '~/components/page/skill/FrontendArea.vue'
import BackendArea from '~/components/page/skill/BackendArea.vue'
import ToolArea from '~/components/page/skill/ToolArea.vue'

export default {
  components: {
    FrontendArea,
    BackendArea,
    ToolArea
  }
}
</script>

<style lang="scss" scoped>
.skill {
  > .frontend-area {
    margin-bottom: 50px;
  }
  > .backend-area {
    margin-bottom: 50px;
  }
}
</style>
