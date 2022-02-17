<template>
<div>
    <div class="card">
        <div class="card-body items">
            <slot></slot>
        </div>
    </div>
</div>
</template>

<script>
export default {

}
</script>

<style>
.card-body {
    font-family: 'Arizonia', cursive;
    font-size: 24px;
    color: #6e6e6e;
}
.items {
    cursor: pointer;
}
.items:hover {
    background: #ffe2e2;
}
</style>