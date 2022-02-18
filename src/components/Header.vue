<template>
  <header>
    <Advertising />
    <Navbar />
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
};
</script>

<style></style>
