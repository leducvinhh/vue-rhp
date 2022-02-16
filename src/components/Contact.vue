<template>
  <div>
    <h1>this is Contact page</h1>
    <button @click="count++">Increase Value</button>
    <p>{{ count }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  destroyed() {
    console.log("destroyed contact");
  },
  deactivated() {
    console.log("deactivated contact");
  },
  activated() {
    console.log("activated contact");
  },
  created() {
    console.log("created contact");
  },
};
</script>

<style scoped>
</style>