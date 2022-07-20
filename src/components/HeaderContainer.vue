<template>
  <div class="header-container">
    <div class="title">
      <h2>{{ title }}</h2>
    </div>
    <div class="menu">
      <span class="material-symbols-outlined">menu</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "HeaderContainer",
  props: {
    title: {
      type: String,
      default: "Title",
    },
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "@/assets/styles/variables.scss";

.header-container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 100%;
  height: 86px;
  background-color: map-get($colors, "light-green");

  > .title {
    margin: 0px 10%;
    font-size: 32px;
    font-weight: 500;
    color: map-get($colors, "green");
  }

  > .menu {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 8%;
    height: 30%;
    color: map-get($colors, "green");
    border: 2px solid map-get($colors, "green");
    padding: 1.5%;
    margin-right: 10%;
  }
}
</style>
