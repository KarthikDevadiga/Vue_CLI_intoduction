<template>
  <div class="parent">
    <user-age></user-age>
  </div>
</template>

<script>
import UserAge from "./components/UserAge.vue";
export default {
  name: "App",
  components: [
    {
      UserAge,
    },
  ],
};
</script>

<style></style>
