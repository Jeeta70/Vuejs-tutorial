<!-- Two way binding -->
<!-- It help to bind the variable from model and view -->
<template>
   <h1>Home component</h1>
   <input type="text" v-model="count" /> 
   <h2>{{ count }}</h2>
</template>
<script>
export default {
   name: "HomePage",
   data(){
      return {
         count:10
      }
   }
};
</script>
<style scoped>
h1 {
   color: yellowgreen;
}
</style>
