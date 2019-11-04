<template>
  <article class="carrier-card">
    <h3 class="title">
      <span v-for="item in title" :key="item.id" class="line-group">
        {{ item }}
      </span>
      <span class="period line-group">({{ period }})</span>
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
      type: Array,
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
    :first-child {
      margin-right: 4px;
    }
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
      margin-bottom: 4px;
      > .period {
        font-size: 1.2rem;
      }
    }
    > .paragraph {
      word-break: break-word;
      margin-bottom: 4px;
      padding-right: 0;
    }
  }
}
</style>
