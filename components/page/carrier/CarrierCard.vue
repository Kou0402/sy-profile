<template>
  <article class="carrier-card">
    <h2 class="title">
      {{ title }} <span class="period">(期間：{{ period }}ヶ月)</span>
    </h2>
    <h3 class="subtitle">
      - 概要 -
    </h3>
    <p class="paragraph">
      {{ overview }}
    </p>
    <h3 class="subtitle">
      - 技術 -
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
  > .title {
    font-weight: 500;
    margin-bottom: 8px;
    > .period {
      font-size: 1.6rem;
      font-weight: 600;
    }
  }
  > .subtitle {
    font-size: 1.6rem;
  }
  > .paragraph {
    font-size: 1.6rem;
    margin-bottom: 8px;
  }
}
</style>
