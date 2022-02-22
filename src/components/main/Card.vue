<template>
  <div class="cards">
    <div
      v-for="(instructor, index) in instructors"
      :key="index"
      class="card mx-5"
    >
      <figure>
        <img
          :src="require(`../../assets/img/${instructor.image}`)"
          :alt="instructor.name"
          class="img-fluid"
        />
      </figure>

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
figure {
  padding: 20px;
}

img {
  &:hover {
    box-shadow: 0px 0px 10px 2px $color_gray;
    cursor: pointer;
  }
}

p,
i {
  color: $color_gray;
}
</style>
