<template>
  <article class="carrier-card">
    <h2 class="title">
      {{ title }} <span>（期間：{{ period }}ヶ月）</span>
    </h2>
    <h3 class="subtitle">
      概要
    </h3>
    <p class="paragraph">
      {{ overview }}
    </p>
    <h3 class="subtitle">
      技術
    </h3>
    <p class="paragraph">
      {{ technology }}
    </p>
  </article>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      required: true
    },
    period: {
      type: Number,
      required: true
    },
    overview: {
      type: String,
      required: true
    },
    technology: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.carrier-card {
  color: $main-color1;
  > .title {
    font-size: 3.2rem;
    font-weight: 500;
    margin-bottom: 20px;
  }
  > .subtitle {
    font-size: 2.4rem;
    font-weight: 500;
    margin-bottom: 10px;
  }
  > .paragraph {
    font-size: 1.9rem;
    margin-bottom: 17px;
  }
}
</style>
