<template>
    <div id="app">
        <div class="container">
            <div class="row">
                <div class="col-sm-12">
                    <card cardWords="test">
                        <h2>{{ title }}</h2>
                        <p>White card is so ugli!</p>
                    </card>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import Card from './components/Card.vue'

export default {
    components: {
        Card
    },
    data() {
        return {
            title: 'Cart Title'
        }
    }
}
</script>

<style>
</style>
