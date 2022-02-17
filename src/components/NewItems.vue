<template>
  <form action="" id="form-add-todo">
      <label for="add-todo">New Todo</label>
      <input v-model="nameTodo" type="text" name="" id="add-todo">
      <button @click.prevent="addTodo">Add Todo</button>
  </form>
</template>

<script>
export default {
    data() {
        return {
            nameTodo: '',
        }
    },
    methods: {
        addTodo() {
            this.$emit('addTodo', this.nameTodo)
            this.nameTodo = '';
        }
    }
}
</script>

<style>
#form-add-todo {
    display: flex;
    justify-content: center;
    margin: 20px auto;
}
</style>