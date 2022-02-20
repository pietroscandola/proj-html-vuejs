<template>
  <div class="bg-image">
    <div class="container h-100">
      <div class="row h-100 align-items-center">
        <div class="col-6">
          <p>
            &copy; Copyright 2012 - 2020| Avada Theme by
            <span>ThemeFusion</span> | All Rights Reserved | Powered by
            <span>Wordpress</span>
          </p>
        </div>
        <div class="col-6 d-flex justify-content-end">
          <ul class="d-flex">
            <li><i class="fa-brands fa-facebook-f mx-2"></i></li>
            <li><i class="fa-brands fa-twitter mx-2"></i></li>
            <li><i class="fa-brands fa-youtube mx-2"></i></li>
            <li><i class="fa-brands fa-instagram mx-2"></i></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "BottomFooter",
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";
.bg-image {
  min-width: 100%;
  height: 100px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-color: black;
}
p {
  font-size: 13px;
  color: $color_gray;
}

span {
  color: $color_green;
}

li {
  list-style-type: none;
}

.fa-brands {
  font-size: 1.3rem;
  color: white;
}
</style>
