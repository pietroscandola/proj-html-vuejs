<template>
  <section class="bg-image">
    <div class="container h-100">
      <div class="row align-items-center h-100">
        <div class="col-3">
          <img
            src="../../assets/img/avada-drivers-logo-1x.png"
            alt="Logo Avada"
          />
          <p>
            Avada Driving School is the right choice for experienced drivers
            looking for a refrescher course, or the brand new driver wanting to
            pass first time
          </p>
        </div>
        <div class="col-3">
          <h4>CONTACT DETAILS</h4>
          <ul>
            <li><i class="fa-solid fa-house-chimney"></i></li>
            <li><i class="fa-solid fa-phone-flip"></i></li>
            <li><i class="fa-solid fa-envelope"></i></li>
            <li></li>
          </ul>
        </div>
        <div class="col-3">
          <h4>CONTACT DETAILS</h4>
          <ul>
            <li><i class="fa-solid fa-circle-arrow-right"></i>Pass Plus</li>
            <li>
              <i class="fa-solid fa-circle-arrow-right"></i>Intensive Course
            </li>
            <li><i class="fa-solid fa-circle-arrow-right"></i>Automatic</li>
            <li>
              <i class="fa-solid fa-circle-arrow-right"></i>Instructor Training
            </li>
          </ul>
        </div>
        <div class="col-3">
          <figure>
            <img src="../../assets/img/footer-ad-grid.png" alt="Advertising" />
          </figure>
          <div>
            <button class="button text-center">BOOK NOW</button>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MainFooter",
};
</script>

<style lang="scss" scoped>
.bg-image {
  background-image: url("../../assets/img/footer-background-color.jpg");
  min-width: 100%;
  height: 400px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
</style>
