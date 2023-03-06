<template>
  <h1>This is child component</h1>
  <p>{{ name }}</p>
  <p>{{ user.name }}</p>
  <button v-on:click="getData()" >Call function</button>
</template>
<script>
export default {
  name: "ChildPage",
  props: {
    name: String,
    user:Object,
    getData:Function
  },
};
</script>
