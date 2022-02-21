<template>
  <section class="container py-5">
    <div class="row">
      <div
        v-for="(rate, index) in rates"
        :key="index"
        :rates="rates"
        class="col-4"
      >
        <CardRate :rate="rate" />
      </div>
    </div>
  </section>
</template>

<script>
import CardRate from "./CardRate.vue";

export default {
  name: "Rate",
  components: {
    CardRate,
  },
  props: ["rates"],
};
</script>

<style scoped>
.card {
  margin-top: -100px;
}
</style>
