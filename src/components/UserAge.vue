<template>
  <div>
    <h1>users age {{ users }}</h1>
    <button @click="incrementAge">increment age</button>
  </div>
</template>

<script>
export default {
  name: "user-age",
  props: ["users"],
  emits: ["user-age-increment"],
  methods: {
    incrementAge() {
      this.$emit("user-age-increment");
    },
  },
};
</script>

<style scoped>
div {
  background-color: #eee;
}
</style>
