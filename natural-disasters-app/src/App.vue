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

<style lang="scss">
*,
*::after,
*::before {
    margin: 0;
    padding: 0;
    box-sizing: inherit;
}
html {
    font-size: 62.5%;
    height: 100%;
}
body {
    box-sizing: border-box;
    height: 100%;
    margin: 3rem;
    background-color: #eeeeee;
}

#app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;

    display: flex;
    flex-direction: column;
    margin: 0;
    padding: 0;

    height: 100%;
}
</style>
