<template>
  <div>
    <h1 v-bind:style="{ 'backgroundColor': bgcolor }">{{ message }}</h1>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      messages: "The quick brown fox jumps over the lazy dog",
    };
  },
  // props act like arguments
  props: ["message", "bgcolor"],
};
</script>

<style scoped>
div {
  background-color: pink;
  text-align: center;
}
</style>