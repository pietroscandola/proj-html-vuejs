<template>
  <div class="bg_ads">
    <div class="container">
      <div class="row py-2">
        <div class="col d-flex align-items-center">
          <span> We have a 95% Successful Pass Rate! </span>
        </div>
        <div class="col d-flex align-items-center justify-content-end">
          <span>Give us a call to book your tuition! 1-800-555-555</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Advertising",
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";

.bg_ads {
  background-color: $bg_ads;
}

span {
  font-size: 12px;
  color: lightgray;
}
</style>
