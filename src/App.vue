<template>
  <div>
    <hello-world :age="age"></hello-world>
    <age :age="age" @increment-age="incrementAge"></age>
    <button @click="age++">plus</button>
    <button @click="age--">minus</button>
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
      age: 21,
    };
  },
  methods: {
    incrementAge() {
      this.age++;
    },
  },
};
</script>
