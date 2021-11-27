<template>
  <div>
    <hello-world></hello-world>
    <age :ge="age"></age>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import age from "./components/age.vue";

export default {
  components: { HelloWorld, age },
  name: "App",
  data() {
    return {
      age: 20,
    };
  },
};
</script>
