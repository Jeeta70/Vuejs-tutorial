<template>
  <h1>Re use component</h1>
  <ul>
    <li v-for="item in users" :key="item.name">
      <User :data="item" :getData="getData" />
    </li>
  </ul>
</template>
<script>
import User from "./User.vue";

export default {
  name: "HomePage",
  data() {
    return {
      users: [
        { name: "Peter", email: "peter@test.com" },
        { name: "Sam", email: "peter@gmail.com" },
        { name: "anil", email: "sam@gmail.com" },
      ],
    };
  },
  methods: {
    getData(name) {
      alert(name)
    },
  },
  components: {
    User,
  },
};
</script>
<style scoped>
h1 {
}
</style>
