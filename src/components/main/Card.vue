<template>
  <div class="cards">
    <div
      v-for="(instructor, index) in instructors"
      :key="index"
      class="card mx-5"
    >
      <img
        :src="require(`../../assets/img/${instructor.image}`)"
        :alt="instructor.name"
      />
      <h5 class="text-center">{{ instructor.name }}</h5>
      <div class="text-center py-1">
        <i class="fa-brands fa-facebook-f px-2"></i>
        <i class="fa-brands fa-twitter px-2"></i>
        <i class="fa-brands fa-instagram px-2"></i>
      </div>
      <p class="text-center p-4">
        Lorem ipsum dolor sit amet consectetur adipisicing elit.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["instructors"],
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";
.cards {
  display: flex;
}

.card {
  border-top: 10px solid $color_green;
  border-radius: 20px;
}

img {
  padding: 20px;
}
p,
i {
  color: $color_gray;
}
</style>
