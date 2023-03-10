<!-- Slot is like this.props.childer in react -->

<template>
  <h1>Slots in vue js 3</h1>
  <Child>
    <h1>Code step by step</h1>
  </Child>
  <Child>
    <a href="#">Code Step Step</a>
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
