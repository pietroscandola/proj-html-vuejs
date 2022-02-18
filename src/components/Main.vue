<template>
  <div>
    <Registration />
    <Phone />
    <Courses />
  </div>
</template>

<script>
import Registration from "./main/Registration.vue";
import Phone from "./main/Phone.vue";
import Courses from "./main/Courses.vue";

export default {
  name: "Main",
  components: {
    Registration,
    Phone,
    Courses,
  },
};
</script>

<style></style>
