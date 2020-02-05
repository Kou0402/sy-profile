<template>
  <section class="skill-description">
    <p>わたしの持っている技術の紹介です。</p>
    <p>『★』の評価基準は以下になります。</p>
    <p>
      <span class="line-group">・★☆☆</span>
      <span class="line-group">
        ：多少触ったことがある。または自主的に勉強している。
      </span>
    </p>
    <p>
      <span class="line-group">・★★☆</span>
      <span class="line-group">
        ：実務で経験している。または自主的に使用している。
      </span>
    </p>
    <p class="last">
      <span class="line-group">・★★★</span>
      <span class="line-group">
        ：実務や自主開発にて１年以上経験している。
      </span>
    </p>
  </section>
</template>

<style lang="scss" scoped>
@media screen and (max-width: 560px) {
  .skill-description {
    .last {
      padding-right: 10vw;
    }
  }
}
</style>
