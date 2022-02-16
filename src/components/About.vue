<template>
  <div>
    <h1>this is About page</h1>
  </div>
</template>

<script>
export default {
  destroyed() {
    console.log("destroyed about");
  },
  deactivated() {
    console.log("deactivated about");
    console.log("deactivated about");
  },
  activated() {
    console.log("activated about");
  },
  created() {
    console.log("created about");
  },
};
</script>

<style scoped>
</style>