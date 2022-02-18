<template>
  <div>
    <Registration />
    <Phonenumber />
  </div>
</template>

<script>
import Registration from "./main/Registration.vue";
import Phonenumber from "./main/Phonenumber.vue";

export default {
  name: "Main",
  components: {
    Registration,
    Phonenumber,
  },
};
</script>

<style></style>
