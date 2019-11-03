<template>
  <section class="skill">
    <h1 class="title">所持スキル</h1>
    <SkillDescription></SkillDescription>
    <FrontendArea></FrontendArea>
    <BackendArea></BackendArea>
    <ToolArea></ToolArea>
  </section>
</template>

<script>
import SkillDescription from '~/components/page/skill/SkillDescription.vue'
import FrontendArea from '~/components/page/skill/FrontendArea.vue'
import BackendArea from '~/components/page/skill/BackendArea.vue'
import ToolArea from '~/components/page/skill/ToolArea.vue'

export default {
  components: {
    SkillDescription,
    FrontendArea,
    BackendArea,
    ToolArea
  }
}
</script>

<style lang="scss" scoped>
.skill {
  > .title {
    color: $main-color1;
    font-size: 3rem;
    font-weight: 500;
    margin-bottom: 30px;
  }
  > .skill-description {
    margin-bottom: 30px;
  }
  > .frontend-area {
    margin-bottom: 50px;
  }
  > .backend-area {
    margin-bottom: 50px;
  }
}
</style>
