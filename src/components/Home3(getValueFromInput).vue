<template>
   <h1>Get input field value</h1>
   <input type="text" placeholder="Enter email" v-model="email" />
   <br />
   <br />
   <input type="text" placeholder="Enter password" v-model="password" />
   <br />
   <br />
   <button v-on:click="getData()" type="button">Get Values</button>
</template>
<script>
export default {
   name: "HomePage",
   data(){
      return{
         email:null,
         password:null
      }
   },
   methods:{
      getData(){
         console.warn("value : ",this.email,this.password)
      }
   }
};
</script>
<style scoped>
h1 {
   color: yellowgreen;
}
</style>
