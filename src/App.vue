<template>
  <div id="app">
    <HeaderContainer title="Foodies" />
  </div>
</template>

<script>
import HeaderContainer from "@/components/HeaderContainer.vue";
export default {
  name: "App",
  components: {
    HeaderContainer,
  },
};
</script>

<style lang="scss">
@import "@/assets/styles/all.scss";

#app {
  font-family: "Inter", sans-serif;
}
</style>
