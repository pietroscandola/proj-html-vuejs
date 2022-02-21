<template>
  <div>
    <Header :navbaritems="navbaritems" />
    <Main
      :instructors="instructors"
      :testimonials="testimonials"
      :rates="rates"
    />
    <Footer :contacts="contacts" :courses="courses" />
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
      rates: [
        {
          percentage: 90,
          name: "PASS RATE",
        },
        {
          percentage: 100,
          name: "REFERRAL RATE",
        },
        {
          percentage: 0,
          name: "ACCIDENT RATE",
        },
      ],
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

      contacts: [
        {
          icon: "fa-solid fa-house-chimney",
          info: "12345 North Main Street, New York, NY 555555",
        },
        {
          icon: "fa-solid fa-phone-flip",
          info: "1.800.555.6789",
        },
        {
          icon: "fa-solid fa-envelope",
          info: "info@your-domain.com",
        },
        {
          icon: "fa-solid fa-link",
          info: "Theme-Fusion",
        },
      ],

      courses: [
        {
          icon: "fa-solid fa-circle-arrow-right",
          info: "Pass Plus",
        },
        {
          icon: "fa-solid fa-circle-arrow-right",
          info: "Intensive Course",
        },
        {
          icon: "fa-solid fa-circle-arrow-right",
          info: "Automatic",
        },
        {
          icon: "fa-solid fa-circle-arrow-right",
          info: "Instructor Training",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "assets/scss/style.scss";
</style>
