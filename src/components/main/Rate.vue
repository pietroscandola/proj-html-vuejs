<template>
  <section class="container py-5">
    <div class="row">
      <div class="col-4"><Card90 /></div>
      <div class="col-4"><Card100 /></div>
      <div class="col-4"><Card /></div>
    </div>
  </section>
</template>

<script>
import Card90 from "./Card_90.vue";
import Card100 from "./Card_100.vue";
import Card from "./Card.vue";

export default {
  name: "Rate",
  components: {
    Card90,
    Card100,
    Card,
  },
};
</script>

<style></style>
