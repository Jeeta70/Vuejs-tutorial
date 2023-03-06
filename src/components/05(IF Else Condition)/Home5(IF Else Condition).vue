<template>
  <h1 v-if="show">If Condition</h1>
  <h1 v-else>Else Condition</h1>

  <button v-on:click="show=!show">Toggle</button>
</template>
<script>
export default {
  name: "HomePage",
  data() {
    return {
      show: false,
    };
  }
};
</script>
<style scoped>
h1 {
  color: yellowgreen;
}
</style>
