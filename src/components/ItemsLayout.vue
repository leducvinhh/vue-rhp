<template>
    <div class="layout">
        <items v-for="(item, index) in items" :key="index">
            <p>{{ item }}</p>
        </items>
    </div>
</template>

<script>
import Items from './Items.vue'
export default {
  components: { Items },
    props: ['items']
}
</script>

<style>

</style>