<template>
  <h1>Form Modifier</h1>
  {{ email }}
<input type="number" v-model.number.lazy="email">
</template>
<script>
export default {
  name: "HomePage",
  data() {
    return {
      email:""
    };
  },
  methods: {
    login() {
      this.error = [];
      for (const item in this.form) {
        if (this.form[item] === "" || this.form[item].length === 0) {
          this.error.push(item);
        }
      }
      if (this.error.length === 0) {
        console.log(this.error);
        alert("Form submitted");
      }
    },
  },
};
</script>
<style>
h1 {
  color: yellow;
}
</style>
