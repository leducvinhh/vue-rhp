<template>
  <div id="app">
    <p v-for="(item, index) in data" :key="index">
      {{ item }}
      <button @click="handleDelete(item)">Delete</button>
    </p>
  </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
  data() {
    return {
      data: ['Cam', 'Buoi', 'Xoai']
    }
  },
  methods: {
    handleDelete(i) {
      this.data = this.data.filter((e) => e !== i )
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
