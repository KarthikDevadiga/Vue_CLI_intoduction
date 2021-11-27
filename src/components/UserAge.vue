<template>
  <div>
    <h1>users age {{ users }}</h1>
  </div>
</template>

<script>
export default {
  name: "user-age",
  props: ["users"],
};
</script>

<style scoped>
div {
  background-color: #eee;
}
</style>
