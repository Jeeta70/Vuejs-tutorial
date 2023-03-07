<template>
  <h1>No Props data</h1>
  <User data="some data" id="user-cmp" />
</template>
<script>
import User from "./User.vue";

export default {
  name: "HomePage",
  data() {
    return {
      email: "",
    };
  },
  methods: {  },
  components: { User },
};
</script>
<style scoped>
h1 {
  color: yellow;
}
</style>
