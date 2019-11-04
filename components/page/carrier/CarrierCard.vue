<template>
  <article class="carrier-card">
    <h3 class="title">
      {{ title }} <span class="period">({{ period }})</span>
    </h3>
    <h4 class="subtitle">
      - 概要 -
    </h4>
    <p class="paragraph">
      <span v-for="item in overview" :key="item.id" class="line-group">
        {{ item }}
      </span>
    </p>
    <h4 class="subtitle">
      - 技術 -
    </h4>
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
      type: Array,
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
  .line-group {
    margin-right: 0;
  }
  > .title {
    margin-bottom: 8px;
    > .period {
      font-size: 1.6rem;
    }
  }
  > .paragraph {
    margin-bottom: 8px;
    padding-right: 18vw;
  }
}

@media screen and (max-width: 560px) {
  .carrier-card {
    > .title {
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
