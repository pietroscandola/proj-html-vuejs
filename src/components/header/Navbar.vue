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
          <nav class="pt-3">
            <ul class="d-flex justify-content-around align-items-center">
              <li
                v-for="(navbaritem, index) in navbaritems"
                :key="index"
                @click="setIndex(index)"
              >
                <a href="#" :class="{ active: isActive(index) }">{{
                  navbaritem
                }}</a>
              </li>
              <li><a href="#" class="button">BOOK NOW</a></li>
            </ul>
          </nav>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  props: ["navbaritems"],
  data() {
    return {
      currentIndex: 0,
    };
  },
  methods: {
    isActive(index) {
      return index === this.currentIndex;
    },
    setIndex(index) {
      this.currentIndex = index;
    },
  },
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
}
.active {
  color: $color_green;
  border-bottom: 3px solid $color_green;
}

li {
  list-style-type: none;
}
</style>
