<template>
  <p>user's {{ age }}</p>
  <button @click="incrementAge">age++</button>
</template>

<script>
export default {
  name: "age",
  props: ["age"],
  emits: ["increment-age"],
  methods: {
    incrementAge() {
      this.$emit("increment-age");
    },
  },
};
</script>

<style scoped>
button {
  background-color: transparent;
  border-color: red;
}
</style>
