<template>
  <div>
    <Header :navbaritems="navbaritems" />
    <Main :instructors="instructors" :testimonials="testimonials" />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Main,
    Footer,
  },
  data() {
    return {
      navbaritems: ["HOME", "ABOUT", "PRICES", "COURSES", "LOCATION", "BLOG"],
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
          name: "Grant Harvey",
          image: "testimonial-grant.png",
        },
        {
          id: 2,
          name: "Harold Green",
          image: "testimonial-harold.png",
        },
        {
          id: 3,
          name: "Kate Lewis",
          image: "testimonial-kate.png",
        },
        {
          id: 4,
          name: "Kelly Johnson",
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
