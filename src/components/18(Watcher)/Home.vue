<!-- Watcher is like a React useEffect with dipendency array -->
<template>
  <h1>Watchers</h1>
  <h2>{{ count }}</h2>
  <button v-on:click="count = count + 1">+</button>
  <button v-on:click="count = count - 1">-</button>
</template>
<script>
export default {
  name: "HomePage",
  data() {
    return {
      count: 0,
    };
  },
  watch:{
    count(val,prev){
      console.log(val,prev)
      if(val >5){
        alert("stop counting")
      }
    }
  },
};
</script>
<style scoped>
h1 {
  color: green;
}
</style>
