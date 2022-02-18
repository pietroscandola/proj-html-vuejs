<template>
  <div class="bg-navbar">
    <div class="container">
      <div class="row py-4">
        <div class="col-3">
          <figure>
            <img
              src="../../assets/img/avada-drivers-logo-1x.png"
              alt="Logo avada"
            />
          </figure>
        </div>
        <div class="col-9">
          <nav class="py-2">
            <div class="row align-items-center justify-content-between">
              <div class="col-1 d-flex align-items-center justify-content-end">
                <a href="#" class="active">HOME</a>
              </div>
              <div class="col-1 d-flex align-items-center justify-content-end">
                <a href="#">ABOUT</a>
              </div>
              <div class="col-1 d-flex align-items-center justify-content-end">
                <a href="#">PRICES</a>
              </div>
              <div class="col-1 d-flex align-items-center justify-content-end">
                <a href="#">COURSES</a>
              </div>
              <div class="col-1 d-flex align-items-center justify-content-end">
                <a href="#">LOCATION</a>
              </div>
              <div class="col-1 d-flex align-items-center justify-content-end">
                <a href="#">BLOG</a>
              </div>
              <div class="col-2 d-flex align-items-center justify-content-end">
                <a href="#" class="button">BOOK NOW</a>
              </div>
            </div>
          </nav>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";

.bg-navbar {
  background-color: $bg_navbar;
  position: fixed;
  width: 100%;
  top: 34px;
  z-index: 1;
}

a {
  color: white;
  font-weight: 600;
  padding-bottom: 5px;
  text-decoration: none;
}

a:hover {
  color: $color_green;
  border-bottom: 1px solid $color_green;
}

.active {
  color: $color_green;

  border-bottom: 1px solid $color_green;
}
</style>
