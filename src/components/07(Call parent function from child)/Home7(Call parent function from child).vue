<template>
  <h1>For loop in vue</h1>
  <Child name="anil sidhu" :user="user" :getData="getData" />
</template>
<script>
import Child from "./Child.vue";

export default {
  name: "HomePage",
  data(){
    return{
      user:{name:"Peter",email:"peter@test.com"}
    }
  },
  methods:{
    getData(){
      console.log('parent function called')
    }
  },
  components: {
    Child,
  },
};
</script>
<style scoped>
h1 {
}
</style>
