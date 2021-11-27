<template>
  <div>
    <h1>users age {{ users }}</h1>
    <button @click="checking">check</button>
  </div>
</template>

<script>
export default {
  name: "user-age",
  props: {
    users: {
      type: Number,
      required: true,
      default: 20,
      validator(value) {
        return value < 100;
      },
    },
  },
  methods: {
    checking() {
      console.log(this.$props.users);
    },
  },
};
</script>

<style scoped>
div {
  background-color: #eee;
}
</style>
