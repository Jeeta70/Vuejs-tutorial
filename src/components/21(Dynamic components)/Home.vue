
<!-- Dynamic component means load different component on basis of condition without using if else -->
<template>
  <h1>Dynamic components</h1>
  <Button @click = "tab = 'java'" >Load Java</Button>
  <Button @click = "tab = 'node'">Load Node</Button>
  <Button @click = "tab = 'php'" >Load Php</Button>
  <component :is="tab" />
</template>
<script>
import Java from "./Java.vue";
import Node from "./Node.vue";
import Php from "./Php.vue";

export default {
  name: "HomePage",
  components: { Java, Node, Php },
  data() {
    return {
      tab: "Node",
    };
  },
};
</script>
<style scoped>
h1 {
  color: green;
}
</style>
