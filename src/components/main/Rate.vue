<template>
  <section class="container py-5">
    <div class="row">
      <div class="col-4"><Card90 /></div>
      <div class="col-4"><Card100 /></div>
      <div class="col-4"><Card0 /></div>
    </div>
  </section>
</template>

<script>
import Card90 from "./Card_90.vue";
import Card100 from "./Card_100.vue";
import Card0 from "./Card_0.vue";

export default {
  name: "Rate",
  components: {
    Card90,
    Card100,
    Card0,
  },
};
</script>

<style scoped>
.card {
  margin-top: -100px;
}
</style>
