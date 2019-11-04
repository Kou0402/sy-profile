<template>
  <div class="nav-link">
    <nuxt-link :to="path" class="name"><slot></slot></nuxt-link>
  </div>
</template>

<script>
export default {
  props: {
    path: {
      type: String,
      required: true
    }
  }
}
</script>

<style lang="scss" scoped>
.nav-link {
  > .name {
    display: inline-block;
    color: $main-color1;
    position: relative;
    font-size: 2.4rem;
    text-decoration: none;
  }
  > .name::after {
    position: absolute;
    bottom: -8px;
    left: 0;
    content: '';
    background: $main-color1;
    width: 100%;
    height: 1px;
    transform: scale(0, 1);
    transform-origin: center top;
    transition: transform 0.3s;
  }
  > .name:hover::after {
    transform: scale(1, 1);
  }
  > .nuxt-link-exact-active::after {
    position: absolute;
    bottom: -8px;
    left: 0;
    content: '';
    width: 100%;
    height: 1px;
    background: $main-color1;
    transform: scale(1, 1);
    transform-origin: center top;
  }
}

@media screen and (max-width: 560px) {
  .nav-link {
    > .name {
      font-size: 1.6rem;
    }
  }
}
</style>
