<template>
  <h1 :class="applyStyle">{{ text }}</h1>
  <button v-on:click="colorfull = !colorfull">Add style</button>
</template>
<script>
export default {
  name: "HomePage",
  data() {
    return {
      text: "Anil sidhu",
      colorfull: false,
    };
  },
  computed: {
    applyStyle() {
      return { green: this.colorfull, err: true,other:false  };
    },
  },
};
</script>
<style scoped>
.green {
  background-color: green;
}

.err {
  color: red;
}
.other{
   text-decoration: underline;
}
</style>
