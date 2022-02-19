<template>
  <div class="card">
    <div class="flex-wrapper py-5">
      <div class="single-chart">
        <svg viewBox="0 0 36 36" class="circular-chart blue">
          <path
            class="circle-bg"
            d="M18 2.0845
          a 15.9155 15.9155 0 0 1 0 31.831
          a 15.9155 15.9155 0 0 1 0 -31.831"
          />
          <path
            class="circle"
            stroke-dasharray="90, 100"
            d="M18 2.0845
          a 15.9155 15.9155 0 0 1 0 31.831
          a 15.9155 15.9155 0 0 1 0 -31.831"
          />
          <text x="18" y="20.35" class="percentage">90%</text>
        </svg>
      </div>
    </div>
    <h5 class="text-center pb-5">PASS RATE</h5>
  </div>
</template>

<script>
export default {
  name: "Card90",
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";

.card {
  border-top: 10px solid $color_green;
  border-radius: 20px;
}

.flex-wrapper {
  display: flex;
  flex-flow: row nowrap;
}

.single-chart {
  width: 100%;
  justify-content: space-around;
}

.circular-chart {
  display: block;
  margin: 10px auto;
  max-width: 80%;
  max-height: 250px;
}

.circle-bg {
  fill: none;
  stroke: #eee;
  stroke-width: 2.5;
}

.circle {
  fill: none;
  stroke-width: 1.5;
  stroke-linecap: round;
  animation: progress 3s ease-out forwards;
}

@keyframes progress {
  0% {
    stroke-dasharray: 0 100;
  }
}

.circular-chart.blue .circle {
  stroke: $color_green;
}

.percentage {
  fill: #666;
  font-family: sans-serif;
  font-size: 0.5em;
  text-anchor: middle;
}
</style>
