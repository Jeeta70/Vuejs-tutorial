<template>
  <h1>Ref in vue js</h1>
  <input type="text" ref="input" />
  <button v-on:click="getData">Click me</button>
</template>
<script>
export default {
  name: "HomePage",
  data() {
    return {
      childUser: "John",
    };
  },
  methods: {
    getData() {
      this.$refs.input.focus();
      console.warn(this.$refs.input.value);
    },
  },
};
</script>
<style></style>
