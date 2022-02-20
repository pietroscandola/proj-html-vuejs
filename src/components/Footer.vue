<template>
  <div>
    <MainFooter />
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
};
</script>

<style></style>
