<template>
  <h1>Send data(Child to Parent)</h1>
  <h1>{{ childUser }}</h1>
  <User :getUser="getUserName" />
</template>
<script>
import User from "./User.vue";

export default {
  name: "HomePage",
  components: {
    User,
  },
  data() {
    return {
      childUser: "John",
    };
  },
  methods: {
    getUserName(name) {
      this.childUser = name;
    },
  },
};
</script>
<style></style>
