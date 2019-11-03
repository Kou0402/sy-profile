<template>
  <section class="frontend-area">
    <h3 class="title">フロントエンド</h3>
    <div class="skill">
      <SkillCard font-awesome="far fa-file-code" size="4" star="★★★">
        HTML5/CSS3
      </SkillCard>
      <SkillCard font-awesome="fab fa-js-square" size="4" star="★★★">
        JavaScript
      </SkillCard>
      <SkillCard image-file-name="jquery_icon" size="4" star="★★★">
        jQuery
      </SkillCard>
      <SkillCard font-awesome="fab fa-vuejs" size="4" star="★★☆">
        Vue.js
      </SkillCard>
      <SkillCard image-file-name="nuxt_icon" size="4" star="★★☆">
        Nuxt.js
      </SkillCard>
    </div>
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
.frontend-area {
  > .skill {
    display: flex;
    width: 800px;
    height: 270px;
    flex-direction: column;
    flex-wrap: wrap;
    > .skill-card {
      margin: 10px 0;
    }
  }
}
</style>
