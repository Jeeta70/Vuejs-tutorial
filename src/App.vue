<template>
  <HelloWorld msg="This is hello world page" />
  <Home />
</template>

<script>
import Home from "./components/Home.vue";
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    Home,
    HelloWorld,
  },
};
</script>

