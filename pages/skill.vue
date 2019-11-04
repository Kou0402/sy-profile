<template>
  <section class="skill">
    <h2 class="title">所持スキル</h2>
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
    font-weight: 500;
    margin-bottom: 16px;
  }
  > .skill-description {
    margin-bottom: 33px;
  }
  > .frontend-area {
    margin-bottom: 32px;
  }
  > .backend-area {
    margin-bottom: 32px;
  }
}

@media screen and (max-width: 560px) {
  .skill {
    > .title {
      font-size: 2rem;
    }
  }
}
</style>
