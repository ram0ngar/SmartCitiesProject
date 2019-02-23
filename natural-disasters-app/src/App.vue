<template>
  <div id="app">
    <navbar></navbar>
    <landing></landing>
    <foot></foot>
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Landing from "./components/Landing.vue";
import Foot from "./components/Foot.vue";

export default {
    name: "app",
    components: {
        Navbar,
        Landing,
        Foot
    }
};
</script>

<style>
#app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
}
</style>
