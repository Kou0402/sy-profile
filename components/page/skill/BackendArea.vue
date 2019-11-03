<template>
  <section class="backend-area">
    <h3 class="title">バックエンド</h3>
    <div class="skill">
      <SkillCard font-awesome="fab fa-java" size="4" star="★★☆">
        Java
      </SkillCard>
      <SkillCard image-file-name="spring_icon" size="4" star="★☆☆">
        Spring
      </SkillCard>
      <SkillCard font-awesome="fab fa-php" size="4" star="★☆☆">
        PHP
      </SkillCard>
      <SkillCard font-awesome="fab fa-laravel" size="4" star="★☆☆">
        Laravel
      </SkillCard>
      <SkillCard image-file-name="database_icon" size="4" star="★★☆">
        SQL
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
.backend-area {
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
