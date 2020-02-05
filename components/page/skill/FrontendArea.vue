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
      <SkillCard image-file-name="typescript_icon" size="4" star="★☆☆">
        TypeScript
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
      <SkillCard image-file-name="angular_icon" size="4" star="★☆☆">
        Angular
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
    width: 72vw;
    max-width: 800px;
    height: 340px;
    flex-direction: column;
    flex-wrap: wrap;
    > .skill-card {
      margin: 10px 0;
    }
  }
}

@media screen and (max-width: 560px) {
  .frontend-area {
    > .skill {
      display: initial;
      > .skill-card {
        margin: 10px 0;
      }
    }
  }
}
</style>
