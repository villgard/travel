<template>
  <div id="app">
    <AppHeader/>
    <AppScreenPrime/>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader";
import AppScreenPrime from "@/components/AppScreenPrime";

export default {
  name: 'App',
  components: {
    AppHeader,
    AppScreenPrime
  }
}
</script>

<style lang="scss">
@import "./assets/styles/main";
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&family=Mulish:wght@300;400;700&family=Playfair+Display:wght@700&display=swap');

#app {
  margin: 0 auto;
  max-width: 1220px;
}
</style>
