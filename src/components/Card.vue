<template>
  <div class="card-vocab">
      <slot></slot>
  </div>
</template>

<script>
export default {
    name: 'Card',
}
</script>

<style scoped>
.card-vocab {
    width: 100%;
    border: 1px solid #ccc;
    box-shadow: 1px 1px 2px #00000099;
    padding: 30px;
    margin: 20px auto;
    text-align: center;
}
h2 {
    color: red;
}
</style>