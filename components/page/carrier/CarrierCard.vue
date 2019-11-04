<template>
  <article class="carrier-card">
    <h2 class="title">
      {{ title }} <span class="period">({{ period }})</span>
    </h2>
    <h3 class="subtitle">
      - 概要 -
    </h3>
    <p class="paragraph" v-html="overview"></p>
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
      type: String,
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
    margin-bottom: 16px;
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

@media screen and (max-width: 560px) {
  .carrier-card {
    > .title {
      font-size: 2rem;
      > .period {
        font-size: 1.4rem;
      }
    }
    > .subtitle {
      font-size: 1.2rem;
    }
    > .paragraph {
      word-break: break-word;
      font-size: 1.2rem;
    }
  }
}
</style>
