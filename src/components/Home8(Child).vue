<template>
  <h2>{{ data.name }}</h2>
  <h2>{{ data.email }}</h2>
  <button v-on:click="getData(data.name)">Alert Name</button>
</template>
<script>
export default {
  name: "User",
  props: { data: Object, getData: Function },
  methods: {
    alertData(name) {
      alert(name);
    },
  },
};
</script>
