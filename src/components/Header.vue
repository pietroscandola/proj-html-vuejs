<template>
  <header>
    <Advertising />
    <Navbar />
    <Jumbotron />
  </header>
</template>

<script>
import Advertising from "./Advertising.vue";
import Navbar from "./Navbar.vue";
import Jumbotron from "./Jumbotron.vue";
export default {
  name: "Header",
  components: {
    Advertising,
    Navbar,
    Jumbotron,
  },
};
</script>

<style></style>
