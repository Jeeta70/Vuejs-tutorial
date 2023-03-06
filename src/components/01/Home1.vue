<!-- Interpolation -->
<template>
   <h1 v-on:mousemove="mousemove()">Home component</h1>
   <button v-on:click="getData('Button 1 clicked')">Click Me</button>
   <button v-on:dblclick="getData('Button double clicked')">Click Me</button>
   <h2>{{ count }}</h2>
</template>
<script>
export default {
   name: "HomePage",
   data(){
      return {
         count:0
      }
   },
   methods:{
      mousemove:function(){
         console.log("mouse is moving")
      },
      getData:function(){
         this.count +=1;
      }
   }
};
</script>
<style scoped>
h1 {
   color: yellowgreen;
}
</style>
