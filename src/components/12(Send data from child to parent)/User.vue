<template>
   <div>User</div>
   <button v-on:click="getUser(userName)">Send User Name</button>
</template>
<script>
export default {
   name: "User",
   data() {
      return {
         userName: "Peter",
      };
   },
   props: {
      getUser: Function,
   },
};
</script>
