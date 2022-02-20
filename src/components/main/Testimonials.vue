<template>
  <section class="bg-image">
    <!-- <div class="container h-100">
      <div class="row h-100">
        <div
          class="col d-flex flex-column justify-content-center align-items-center"
        >
          <h2>Testimonials</h2>
          <p>Here's what our happy drivers had to say about our services:</p>
          <img
            class="py-3"
            v-for="(testimonial, index) in testimonials"
            :key="index"
            :src="require(`../../assets/img/${testimonial.image}`)"
            :alt="testimonial.name"
          />
          <p class="text-center">
            Avada Driving School really helped build my confidence behind the
            wheel and with driving in general, and they got me a first time
            pass! Highly recommended.
          </p>
        </div>
      </div>

      <div class="slider d-flex align-items-center">
        <div class="slider-dots">
          <div
            v-for="(testimonial, index) in testimonials"
            :key="index"
            class="dot mx-2"
            @click="this.currentIndex = index"
          ></div>
        </div>
      </div>
    </div> -->
  </section>
</template>

<script>
export default {
  name: "Testimonials",
  props: ["testimonials"],
  data() {
    return {
      currentIndex: 0,
    };
  },
};
</script>

<style lang="scss" scoped>
.bg-image {
  min-width: 100%;
  height: 900px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-image: url("../../assets/img/testimonial-background.jpg");
  margin-top: -100px;
}

p {
  padding: 0 100px;
}

img {
  width: 15%;
}

.slider {
  height: 500px;
  position: relative;
}

.slider .slider-dots {
  padding: 5px;
  border-radius: 20px;
  display: flex;
  position: absolute;
  top: 100%;
  left: 50%;

  transform: translateX(-50%);
}

.slider-dots .dot {
  height: 20px;
  width: 20px;
  border-radius: 50%;
  background-color: white;
  border: 1px solid rgba(0, 0, 0, 0.3);
  cursor: pointer;
}

.slider-dots .dot.active {
  background-color: rgba(0, 0, 0, 0.3);
}
</style>
