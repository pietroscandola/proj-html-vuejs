<template>
  <div>
    <Registration />
    <Phone />
    <Courses />
    <Rate :rates="rates" />
    <Instructors :instructors="instructors" />
    <Testimonials :testimonials="testimonials" />
    <News :news="news" />
    <Newsletter />
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
import Newsletter from "./main/Newsletter.vue";

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
    Newsletter,
  },
  props: ["instructors", "testimonials", "rates", "news"],
};
</script>

<style></style>
