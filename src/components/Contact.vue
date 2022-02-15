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
        }
    },
    destroyed() {
        console.log('destroyed');
    },
    deactivated() {
        console.log('deactivated');
    },
    activated() {
        console.log('activated');
    }
};
</script>

<style scoped>
</style>