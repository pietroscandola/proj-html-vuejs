<template>
  <header>
    <Advertising />
    <Navbar />
  </header>
</template>

<script>
import Advertising from "./Advertising.vue";
import Navbar from "./Navbar.vue";
export default {
  name: "Header",
  components: {
    Advertising,
    Navbar,
  },
};
</script>

<style></style>
