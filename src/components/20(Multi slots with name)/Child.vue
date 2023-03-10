<template>
  <div class="cart">
    <header><slot name="header"></slot></header>
    <content><slot name="main"></slot></content>
    <footer><slot name="footer"><button>B</button></slot></footer>
  </div>
</template>
<script>
export default {
  name: "Child",
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: content-box;
}
div {
  border: 1px solid red;
  width: 30%;
  text-align: center;
}
div:hover footer {
  transform: scale(2);
  transition: all 1s;
}
</style>
