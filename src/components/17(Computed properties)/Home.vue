<!-- Computed properties are used when we want to use complex properties
We can also used normal function but the advantages of using computed properties is that it is fast because it store result in cache -->
<template>
  <h1>Computed properties</h1>
  <h2>{{ dollars * rupeeVal - discount }}</h2>
  <h2>{{ dollars * rupeeVal - discount }}</h2>
  <h2>{{ getResults() }}</h2>
  <h2>{{ getResult }}</h2>
</template>
<script>
export default {
  name: "HomePage",
  data() {
    return {
      dollars: 100,
      rupeeVal: 70,
      discount: 10,
    };
  },
  methods: {
    getResults() {
      return this.dollars * this.rupeeVal - this.discount;
    },
  },
  computed: {
    getResult() {
      return this.dollars * this.rupeeVal - this.discount;
    },
  },
};
</script>
<style scoped>
h1 {
  color: yellow;
}
</style>
