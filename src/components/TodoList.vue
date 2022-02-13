<template>
  <div>
      <p v-if="isShow">{{ title }}</p>
      <button @click="handleClick">Click me</button>
  </div>
</template>

<script>
export default {
    name: 'Todo',
    data() {
        return {
            isShow: true,
            title: 'Hello world'
        }
    },
    methods: {
        handleClick() {
            this.isShow = !this.isShow;
        }
    }
}
</script>

<style>

</style>