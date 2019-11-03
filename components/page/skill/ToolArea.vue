<template>
  <section class="tool-area">
    <h3 class="title">ツール</h3>
    <div class="skill">
      <SkillCard font-awesome="fab fa-windows" size="4" star="★★★">
        Windows
      </SkillCard>
      <SkillCard font-awesome="fab fa-apple" size="4" star="★★☆">
        Mac
      </SkillCard>
      <SkillCard font-awesome="fab fa-linux" size="4" star="★☆☆">
        Linux
      </SkillCard>
      <SkillCard image-file-name="eclipse_icon" size="4" star="★★★">
        Eclipse
      </SkillCard>
      <SkillCard image-file-name="vscode_icon" size="4" star="★★★">
        VSCode
      </SkillCard>
      <SkillCard font-awesome="fab fa-figma" size="4" star="★☆☆">
        Figma
      </SkillCard>
      <SkillCard font-awesome="fas fa-code-branch" size="4" star="★★★">
        SVN
      </SkillCard>
      <SkillCard font-awesome="fab fa-git-square" size="4" star="★★☆">
        Git
      </SkillCard>
      <SkillCard font-awesome="fab fa-github" size="4" star="★★☆">
        GitHub
      </SkillCard>
      <SkillCard image-file-name="circleci_icon" size="4" star="★☆☆">
        CircleCI
      </SkillCard>
      <SkillCard image-file-name="firebase_icon" size="4" star="★★☆">
        Firebase
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
.tool-area {
  > .skill {
    display: flex;
    width: 72vw;
    max-width: 800px;
    height: 540px;
    flex-direction: column;
    flex-wrap: wrap;
    > .skill-card {
      margin: 10px 0;
    }
  }
}
</style>
