<template>
  <h1 v-if="age >= 18">{{ msg }}</h1>
  <h1 v-if="age > 20">get a job!!</h1>
  <h1 v-else>babby</h1>
</template>

<script>
export default {
  name: "hello world",
  props: ["age"],
  data() {
    return {
      msg: "HELLO WORLD",
    };
  },
};
</script>
