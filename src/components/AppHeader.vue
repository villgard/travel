<template>
    <div class="header">
      <AppLogo/>
      <AppButton state="active">Home</AppButton>
      <AppButton>Destinations</AppButton>
      <AppButton>About</AppButton>
      <AppButton>Partner</AppButton>
      <AppButton state="bordered">Login</AppButton>
      <AppButton state="filled">Register</AppButton>
    </div>
</template>

<script>
import AppButton from "@/components/AppButton";
import AppLogo from "@/components/AppLogo";

export default {
name: "AppHeader",
  components: {
    AppButton,
    AppLogo
  },
}
</script>

<style lang="scss">
.header {
  display: flex;
  align-items: center;
  margin-top: 45px;
&__logo{
  margin-right: auto;
  }
}
</style>
