<template>
  <section class="bg-image">
    <div class="container h-100">
      <div class="row">
        <div
          class="col-12 d-flex flex-column justify-content-center align-items-center"
        >
          <h2>Testimonials</h2>
          <p>Here's what our happy drivers had to say about our services:</p>
          <figure
            v-for="(testimonial, index) in testimonials"
            :key="index"
            class="d-flex justify-content-center"
          >
            <img
              class="py-3"
              :src="require(`../../assets/img/${testimonial.image}`)"
              :alt="testimonial.name"
              v-if="isActive(index)"
            />
          </figure>

          <p class="text-center">
            Avada Driving School really helped build my confidence behind the
            wheel and with driving in general, and they got me a first time
            pass! Highly recommended.
          </p>
        </div>

        <div
          v-for="(testimonial, index) in testimonials"
          :key="index"
          class="col-12"
        >
          <h5 v-if="isActive(index)" class="text-center py-3">
            {{ testimonial.name }}
          </h5>
        </div>

        <div class="col-12">
          <div class="slider d-flex align-items-center justify-content-center">
            <div class="slider-dots">
              <div
                v-for="(testimonial, index) in testimonials"
                :key="index"
                class="dot mx-2"
                :class="{ active: isActive(index) }"
                @click="setIndex(index)"
              ></div>
            </div>
          </div>
        </div>
      </div>
    </div>
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
  methods: {
    isActive(index) {
      return index === this.currentIndex;
    },
    setIndex(index) {
      this.currentIndex = index;
    },
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
  padding: 0 150px;
}
img {
  width: 50%;
}

.slider .slider-dots {
  padding: 5px;
  border-radius: 20px;
  display: flex;
}

.slider-dots .dot {
  height: 15px;
  width: 15px;
  border-radius: 50%;
  background-color: white;
  border: 1px solid rgba(0, 0, 0, 0.3);
  cursor: pointer;
}

.slider-dots .dot.active {
  background-color: rgba(0, 0, 0, 0.3);
}

.row {
  padding-top: 100px;
}
</style>
