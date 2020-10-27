<template>
<div :class=" ['title', `title__${state}` ]">
  <slot />
</div>
</template>

<script>
export default {
name: "AppTitle",
  props: {
  state: {
    type: String,
    default: 'prime'
  }
  }
}

</script>

<style lang="scss">
@import "@/assets/styles/main";

.title {
  font-family: 'Playfair Display', serif;
  font-weight: 700;
  &__prime {
    font-size: 36px;
    line-height: 50px;
  }
}
</style>
