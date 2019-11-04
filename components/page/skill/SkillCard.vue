<template>
  <article class="skill-card">
    <div :style="iconSizeStyle" class="icon">
      <i v-if="fontAwesome" :class="fontAwesome"></i>
      <img v-if="imageFileName" :src="imagePath" />
    </div>
    <p class="name">
      <slot></slot>
    </p>
    <div class="star">
      {{ star }}
    </div>
  </article>
</template>

<script>
export default {
  props: {
    fontAwesome: {
      type: String,
      required: false,
      default: ''
    },
    imageFileName: {
      type: String,
      required: false,
      default: ''
    },
    size: {
      type: String,
      required: true
    },
    star: {
      type: String,
      required: true
    }
  },
  data() {
    return {
      iconSizeStyle: {
        fontSize: this.size + 'rem'
      },
      imagePath: this.imageFileName.length
        ? require('~/assets/image/' + this.imageFileName + '.svg')
        : ''
    }
  }
}
</script>

<style lang="scss" scoped>
.skill-card {
  display: flex;
  height: 64px;
  align-items: center;
  text-align: center;
  > .icon {
    color: $accent-color1;
    width: 50px;
    margin-right: 10px;
  }
  > .name {
    width: 120px;
    margin-right: 10px;
  }
  > .star {
    width: 50px;
  }
}

@media screen and (max-width: 560px) {
  .skill-card {
    height: 56px;
    > .icon {
      width: 40px;
    }
    > .name {
      width: 100px;
      font-size: 1.2rem;
    }
    > .star {
      width: 40px;
      font-size: 1.2rem;
    }
  }
}
</style>
