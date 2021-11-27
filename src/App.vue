<template>
  <div class="parent">
    <user-age :users="age"></user-age>
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
};
</script>

<style></style>
