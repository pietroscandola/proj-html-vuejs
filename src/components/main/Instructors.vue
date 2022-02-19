<template>
  <section class="container">
    <h2 class="py-5">Your Instructors</h2>
    <div class="row pb-5">
      <div class="col-9">
        <p>
          Lorem, ipsum dolor sit amet consectetur adipisicing elit. Perspiciatis
          nisi quas placeat praesentium animi vel repellendus ipsa aliquid
          quibusdam eaque fugit commodi eius blanditiis, error unde quis dolorum
          quam labore.
        </p>
      </div>
      <div class="col-3">
        <button class="button w-100">More about us</button>
      </div>
    </div>
    <div class="row pb-5">
      <div class="col-12">
        <Card :instructors="instructors" />
      </div>
    </div>
  </section>
</template>

<script>
import Card from "./Card.vue";
export default {
  name: "Instructors",
  components: {
    Card,
  },
  props: ["instructors"],
};
</script>

<style lang="scss" scoped>
h2 {
  font-size: 3rem;
}
p {
  font-size: 1.2rem;
}
</style>
