<template>
  <div class="bg-navbar">
    <div class="container">
      <div class="row py-4">
        <div class="col-3">
          <figure>
            <img
              src="../../assets/img/avada-drivers-logo-2x-300x58.png"
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
                <a href="#" id="booking"><button>BOOK NOW</button></a>
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
  opacity: 25%;
}

a {
  text-decoration: none;
  color: white;
  font-weight: 600;
}

a:hover {
  color: $color_green;
  text-decoration: underline;
  text-decoration-color: $color_green;
  text-underline-position: under;
}

.active {
  color: $color_green;
  text-decoration: underline;
  text-underline-position: under;
}

button {
  background-color: $color_green;
  color: white;
  font-weight: 600;
  border-radius: 20px;
  padding: 10px;
}
</style>
