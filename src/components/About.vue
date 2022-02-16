<template>
  <div>
    <h1>this is About page</h1>
  </div>
</template>

<script>
export default {
  beforeCreate() {
    console.log('before created about');
  },
  created() {
    console.log('created about');
  },
  beforeMount() {
    console.log('before mount about');
  },
  mounted() {
    console.log('mounted about');
  },
  beforeUpdate() {
    console.log('before update about');
  },
  updated() {
    console.log('updated about');
  },
  beforeDestroy() {
    console.log('before destroy about');
  },
  destroyed() {
    console.log('destroyed about');
  }
};
</script>

<style scoped>
</style>