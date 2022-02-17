<template>
  <div class="container">
    <new-items @addTodo="addTodo"/>
    <items-layout :items="items"/>
  </div>
</template>

<script>
import ItemsLayout from './components/ItemsLayout.vue'
import NewItems from './components/NewItems.vue'
export default {
  components: { ItemsLayout, NewItems},
  name: 'App',
  data() {
    return {
      items: [
        'I love you',
      ],
      maxItems: 10,
    }
  },
  methods: {
    addTodo(e) {
      this.items.push(e);
    }
  }
}
</script>

<style>

</style>