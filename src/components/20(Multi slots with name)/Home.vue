<template>
  <h1>Multiple slots with name</h1>
  <Child>
    <template v-slot:header>
      <h1>Peter</h1>
    </template>
    <template v-slot:main>
      <p>A Vue js product</p>
    </template>
    <template v-slot:footer>
      <button>Click me</button>
    </template>
  </Child>
  <Child>
    <template v-slot:header>
      <h1>Facebook</h1>
    </template>
    <template v-slot:main>
      <p>A React js product</p>
    </template>
    <template v-slot:footer> </template>
  </Child>
</template>
<script>
import Child from "./Child.vue";

export default {
  name: "HomePage",
  components: { Child },
};
</script>
<style scoped>
h1 {
  color: green;
}
</style>
