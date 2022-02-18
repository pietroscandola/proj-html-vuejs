<template>
  <div class="card py-5">
    <div class="percentage">
      <div class="circle">95%</div>
    </div>
    <h5 class="py-4">Pass Rate</h5>
  </div>
</template>

<script>
export default {
  name: "Card",
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";
.card {
  border-top: 10px solid $color_green;
  display: flex;
  align-items: center;
  border-radius: 20px;
}

.percentage {
  height: 200px;
  width: 200px;
  border-radius: 100%;
  font-size: 3rem;
  background: conic-gradient($color_green 95%, white 5%);
  position: relative;
}

.circle {
  border-radius: 50%;
  height: 180px;
  width: 180px;
  background: white;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
