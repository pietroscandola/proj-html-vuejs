<template>
  <div id="avada" class="jumbotron h-100">
    <div class="container h-100">
      <div class="row h-100 align-items-center">
        <div class="col">
          <h1 class="text-white">Drive with Avada</h1>
          <p class="text-white">
            We offer the finest driving tuition money can buy
          </p>
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
  min-height: 700px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

#avada {
  background-image: url("../assets/img/homepage-hero-background.jpg");
}

h1 {
  font-size: 5rem;
}
p {
  font-size: 2rem;
}
</style>
