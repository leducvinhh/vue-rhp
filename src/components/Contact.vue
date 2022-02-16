<template>
  <div>
    <h1 class="hehe">this is Contact page</h1>
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
  beforeCreate() {
    console.log('before created contact');
  },
  created() {
    console.log('created contact');
  },
  beforeMount() {
    console.log('before mount contact');
  },
  mounted() {
    console.log('mounted contact');
  },
  beforeUpdate() {
    console.log('before update contact');
    this.count --
  },
  updated() {
    console.log('updated contact');
  },
  beforeDestroy() {
    console.log('before destroy contact');
  },
  destroyed() {
    console.log('destroyed contact');
  }
};
</script>

<style scoped>
</style>