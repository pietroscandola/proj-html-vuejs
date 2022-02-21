<template>
  <header>
    <Advertising />
    <Navbar :navbaritems="navbaritems" />
    <Jumbotron />
  </header>
</template>

<script>
import Advertising from "./header/Advertising.vue";
import Navbar from "./header/Navbar.vue";
import Jumbotron from "./header/Jumbotron.vue";
export default {
  name: "Header",
  components: {
    Advertising,
    Navbar,
    Jumbotron,
  },
  props: ["navbaritems"],
};
</script>

<style></style>
