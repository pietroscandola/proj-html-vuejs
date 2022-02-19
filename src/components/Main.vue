<template>
  <div>
    <Registration />
    <Phone />
    <Courses />
    <Rate />
    <Instructors :instructors="instructors" />
  </div>
</template>

<script>
import Registration from "./main/Registration.vue";
import Phone from "./main/Phone.vue";
import Courses from "./main/Courses.vue";
import Rate from "./main/Rate.vue";
import Instructors from "./main/Instructors.vue";

export default {
  name: "Main",
  components: {
    Registration,
    Phone,
    Courses,
    Rate,
    Instructors,
  },
  props: ["instructors"],
};
</script>

<style></style>
