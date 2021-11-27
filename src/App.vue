<template>
  <div class="parent">
    <user-age :users="age" @user-age-increment="incrementAge"></user-age>
  </div>
</template>
/* * here "user-age-increment" is emited from "UserAge" component */
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
    incrementAge() {
      this.age++;
    },
  },
};
</script>

<style></style>
