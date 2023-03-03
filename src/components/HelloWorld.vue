<template>
  <div class="hello">

  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  email:"email@gmail.com",
  data(){
    return {
      email:"abc@gmail.com",
      mobile:9999
    }
  },
  methods:{
    getName(name){
      return name
    },
    getData(){
      return {
        name:"anil",
        email:this.email
      }
    }
  },
  props: {
    msg: String
  }
}
</script>
<style scoped>
  h1{
    color: pink;
  }
</style>

