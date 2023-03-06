

<template>
  <h1>{{ text }}</h1>
  <div v-html="tag"></div>

</template>
<script>

export default {
  name: "HomePage",
  data() {
    return {
     text:"Anil sidhu",
     tag:"<h1>Anil sidhu</h1>"
  }
}
};
</script>
<style scoped>
h1 {
}
</style>
