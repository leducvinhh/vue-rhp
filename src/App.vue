<template>
  <div id="app">
    <div class="container">
      <div class="row">
        <div class="col-sm-12">
          <button class="btn btn-outline-danger" @click="selectedComponent = 'Card'">Card Page</button>
          <button class="btn btn-outline-danger" @click="selectedComponent = 'Contact'">Contact Page</button>
          <button class="btn btn-outline-danger" @click="selectedComponent = 'About'">About Page</button>
        </div>
      </div>
      <div class="row">
        <div class="col-sm-12">
          <keep-alive>
            <component :is="selectedComponent"></component>
          </keep-alive>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import About from './components/About.vue';
import Card from "./components/Card.vue";
import Contact from './components/Contact.vue';

export default {
  components: {
    Card,
    Contact,
    About,
  },
  data() {
    return {
      title: "Cart Title",
      selectedComponent: 'Card'
    };
  },
};
</script>

<style>
</style>
