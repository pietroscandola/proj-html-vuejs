<template>
  <div>
    <Header />
    <Main :instructors="instructors" />
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
    };
  },
};
</script>

<style lang="scss">
@import "assets/scss/style.scss";
</style>
