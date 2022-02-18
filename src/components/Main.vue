<template>
  <div>
    <Registration />
    <Phone />
    <Courses />
    <Rate />
  </div>
</template>

<script>
import Registration from "./main/Registration.vue";
import Phone from "./main/Phone.vue";
import Courses from "./main/Courses.vue";
import Rate from "./main/Rate.vue";

export default {
  name: "Main",
  components: {
    Registration,
    Phone,
    Courses,
    Rate,
  },
};
</script>

<style></style>
