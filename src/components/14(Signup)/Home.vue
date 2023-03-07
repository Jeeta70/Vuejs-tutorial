<template>
  <h1>Simple Form</h1>
  <ul>
    <li v-for="item in error" v-bind:key="item">
      {{item }} not valid
    </li>
  </ul>
  <form>
    <label for="">Email: </label>
    <input type="text" placeholder="Enter email" v-model="form.email" />
    <br />
    <br />
    <label for="">Password: </label>
    <input
      type="password"
      placeholder="Enter password"
      v-model="form.password"
    />
    <br />
    <br />
    <select v-model="form.country">
      <option value="india">India</option>
      <option value="china">China</option>
      <option value="usa">USA</option>
    </select>
    <h3>Technology</h3>
    <label for="">Java: </label>
    <input type="checkbox" value="java" v-model="form.technology" />
    <br />
    <br />
    <label for="">Python: </label>
    <input type="checkbox" value="python" v-model="form.technology" />
    <br />
    <br />
    <h3>Gender</h3>
    <label for="">Male: </label>
    <input type="radio" value="male" name="gender" v-model="form.gender" />
    <br />
    <br />
    <label for="">Female: </label>
    <input type="radio" value="female" name="gender" v-model="form.gender" />
    <br />
    <br />
    <button v-on:click="login" type="button">Login</button>
  </form>
</template>
<script>
export default {
  name: "HomePage",
  data() {
    return {
      form: {
        email: "",
        password: "",
        country: "",
        technology: [],
        gender: "",
      },
      error: [],
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
