<template>
  <button type="button" class="vue-button" />
</template>

<script>
export default {
  name: "VueButton",
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

.vue-button {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
</style>
