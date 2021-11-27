<template>
  <div class="parent">
    <user-age :users="age"></user-age>
    <button @click="increment">increment</button>
  </div>
</template>

<script>
import UserAge from "./components/UserAge.vue";
export default {
  name: "App",
  components: {
    UserAge,
  },
  data() {
    return {
      age: 20,
    };
  },
  methods: {
    increment() {
      this.age += 5;
    },
  },
};
</script>

<style></style>
