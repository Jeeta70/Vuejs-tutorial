<template>
  <h1>Props in vue js</h1>
  <Student :name="name" />
  <Teacher :name="name"/>
</template>
<script>
import Student from "./Student.vue";
import Teacher from "./Teacher.vue";

export default {
  name: "HomePage",
  components: {
    Student,
    Teacher,
  },
  data(){
    return{
      name:"Bruce"
    }
  }
};
</script>
<style></style>
