<template>
  <h1>For loop in vue</h1>
  <ul>
    <li v-for="item in technology" :key="item">
      {{ item }}
    </li>
  </ul>
  <h1>For loop in array of object</h1>
  <ul>
    <li v-for="item in users" :key="item">
      Name is {{ item.name }} and the email is {{ item.email }}
   </li>
  </ul>
</template>
<script>
export default {
  name: "HomePage",
  data() {
    return {
      technology: ["java", "php", "node", "html"],
      users: [
        { name: "Ajeet", email: "ajrana70@gmail.com" },
        { name: "akshay", email: "akshay@gmail.com" },
        { name: "sharukh", email: "sharukh@gmail.com" },
      ],
    };
  },
};
</script>
<style scoped>
h1 {
  color: yellowgreen;
}
</style>
