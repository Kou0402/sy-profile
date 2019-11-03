<template>
  <article class="skill-card">
    <div :style="iconSizeStyle" class="icon">
      <i v-if="fontAwesome" :class="fontAwesome"></i>
      <img v-if="imageFileName" :src="imagePath" />
    </div>
    <h3 class="name">
      <slot></slot>
    </h3>
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
      type: Number,
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
  height: 70px;
  color: $main-color1;
  align-items: center;
  text-align: center;
  > .icon {
    width: 50px;
    margin-right: 10px;
  }
  > .name {
    width: 150px;
    font-size: 2rem;
    margin-right: 10px;
  }
  > .star {
    width: 50px;
    font-size: 1.5rem;
  }
}
</style>
