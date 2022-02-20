<template>
  <div>
    <Registration />
    <Phone />
    <Courses />
    <Rate />
    <Instructors :instructors="instructors" />
    <Testimonials :testimonials="testimonials" />
    <News />
  </div>
</template>

<script>
import Registration from "./main/Registration.vue";
import Phone from "./main/Phone.vue";
import Courses from "./main/Courses.vue";
import Rate from "./main/Rate.vue";
import Instructors from "./main/Instructors.vue";
import Testimonials from "./main/Testimonials.vue";
import News from "./main/News.vue";

export default {
  name: "Main",
  components: {
    Registration,
    Phone,
    Courses,
    Rate,
    Instructors,
    Testimonials,
    News,
  },
  props: ["instructors", "testimonials"],
};
</script>

<style></style>
