<template>
  <section class="backend-area">
    <h2 class="title">バックエンド</h2>
    <SkillCard image-file-name="github_icon">フロント</SkillCard>
  </section>
</template>

<script>
import SkillCard from '~/components/page/skill/SkillCard.vue'

export default {
  components: {
    SkillCard
  }
}
</script>

<style lang="scss" scoped>
.backend-area {
  color: $main-color1;
  > .title {
    font-size: 3rem;
  }
}
</style>
