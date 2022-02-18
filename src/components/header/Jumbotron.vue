<template>
  <div id="avada" class="jumbotron">
    <div class="container h-100">
      <div class="row h-100 align-items-center">
        <div class="col-6">
          <h1 class="text-white">Drive with Avada</h1>
          <p class="text-white">
            We offer the finest driving tuition money can buy
          </p>
        </div>
        <div class="col-6">
          <div class="figure">
            <img src="" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Jumbotron",
};
</script>

<style scoped>
.jumbotron {
  min-width: 100%;
  height: 700px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  padding-top: 146px;
}

#avada {
  background-image: url("../../assets/img/homepage-hero-background.jpg");
}

h1 {
  font-size: 3.5rem;
}
p {
  font-size: 1.5rem;
}
</style>
