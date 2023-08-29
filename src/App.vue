<template>
  <div>
    <p>{{ name }}</p>
    <h2>{{ age }}</h2>
    <button @click="changeName('mo')">change name</button>
    <button @click="changeAge(30)">change Age</button>
  </div>
</template>

<script lang="ts">
let age: string | number = "25";

export default {
  name: "App",
  components: {},
  data() {
    return {
      name: "name",
      age: "Age" as number | string,
    };
  },
  methods: {
    changeName(name: string) {
      this.name = name;
      return name;
    },
    changeAge(age: number) {
      this.age = age;
      return age;
    },
  },
};
</script>
