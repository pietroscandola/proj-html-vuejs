<template>
  <div>
    <Header />
    <Main :instructors="instructors" :testimonials="testimonials" />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
  },
  data() {
    return {
      instructors: [
        {
          name: "Mike Hart",
          image: "instructor-mikehart.jpg",
        },
        {
          name: "John Smith",
          image: "instructor-johnsmith.jpg",
        },
        {
          name: "Angela Hart",
          image: "instructor-angelahart.jpg",
        },
      ],

      testimonials: [
        {
          id: 0,
          name: "Sophia Jones",
          image: "testimonial-sophia.png",
        },
        {
          id: 1,
          name: "Grant",
          image: "testimonial-grant.png",
        },
        {
          id: 2,
          name: "Harold",
          image: "testimonial-harold.png",
        },
        {
          id: 3,
          name: "Kate",
          image: "testimonial-kate.png",
        },
        {
          id: 4,
          name: "Kelly",
          image: "testimonial-kelly.png",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "assets/scss/style.scss";
</style>
