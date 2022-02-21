<template>
  <div>
    <MainFooter :contacts="contacts" :courses="courses" />
    <BottomFooter />
  </div>
</template>

<script>
import MainFooter from "./footer/MainFooter.vue";
import BottomFooter from "./footer/BottomFooter.vue";
export default {
  name: "Footer",
  components: {
    MainFooter,
    BottomFooter,
  },
  props: ["contacts", "courses"],
};
</script>

<style></style>
