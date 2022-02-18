<template>
  <div class="bg-navbar">
    <div class="container">
      <div class="row py-4">
        <div class="col-3">
          <img
            src="../assets/img/avada-drivers-logo-2x-300x58.png"
            alt="Logo avada"
          />
        </div>
        <div class="col-9">
          <nav class="py-2">
            <div class="row align-items-center justify-content-between">
              <div class="col-1 d-flex align-items-center justify-content-end">
                <a href="#">HOME</a>
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
                <a href="#" class="booking">BOOK NOW</a>
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
@import "../assets/scss/style.scss";

.bg-navbar {
  background-color: $bg_navbar;
}
a {
  text-decoration: none;
  color: white;
  font-weight: 600;
}

.booking {
  padding: 15px 20px;
  background-color: #79b27b;
  border-radius: 20px;
}
</style>
