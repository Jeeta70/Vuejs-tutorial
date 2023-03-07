<template>
  <div>
    <h3 v-bind="$attrs">Peter</h3>
    <h3>Bruce</h3>
    <h3>Anil</h3>
    <h3>{{ data }}</h3>
  </div>
</template>
<script>
export default {
  name: "User",
  inheritAttrs: false,
  props: {
    data: String,
  },
};
</script>
