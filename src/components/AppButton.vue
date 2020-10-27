<template>
  <div :class="[ 'button', `button__${state}`]">
    <slot />
  </div>
</template>

<script>
export default {
name: "AppButton",
  props: {
    state: {
      type: String,
      default: 'transparent'
    }
  }
}
</script>

<style lang="scss">
@import "@/assets/styles/main";
.button {
  border-radius: 8px;
  font-size: $s;
  font-family: "Inter", sans-serif;
  cursor: pointer;
  &__active {
    color: $black-1;
  }
  &__transparent {
    color: #E5E5E5;
    margin-left: 34px;
    &:hover {
      color: #202336;
      transition: 0.2s;
    }
  }
  &__bordered {
    border: 1px solid $orange;
    color: $orange;
    padding: 15px 46px;
    margin-left: 34px;
    margin-right: 18px;
    font-size: $xs;
  }
  &__filled {
    background-color: $orange;
    border: 1px solid $orange;
    color: $white;
    padding: 15px 36px;
    font-size: $xs;
  }
}
</style>
