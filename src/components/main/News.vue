<template>
  <section class="bg-image">
    <div class="container">
      <div class="card-news">
        <div class="card">
          <h2 class="text-center py-5">Latest News</h2>
          <div class="row d-flex">
            <div
              v-for="(news, index) in news"
              :key="index"
              class="col-6 d-flex flex-column justify-content-center align-items-center"
            >
              <img
                :src="require(`../../assets/img/${news.image}`)"
                alt="Blog Choose Car"
              />
              <h5 class="pt-4">{{ news.title }}</h5>
              <p class="font-12">Februar 7th,2019 | <span>0 Comments</span></p>
              <p class="py-2">
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
              </p>
            </div>
          </div>
          <div class="d-flex justify-content-center">
            <button class="button my-5">MORE FROM THE BLOG</button>
          </div>
        </div>
        <div>
          <img
            class="latestnews-bottom"
            src="../../assets/img/latestnews-bottom.png"
            alt="latestnews-bottom"
            id="latestnews-bottom"
          />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "News",
  props: ["news"],
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";

.bg-image {
  min-width: 100%;
  height: 900px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  background-image: url("../../assets/img/latestnews-background.jpg");
}
h2 {
  font-size: 3rem;
}

h5 {
  color: $color_green;
}

.font-12 {
  font-size: 12px;
}

.card-news {
  position: relative;
  top: -50px;
}

.card {
  border-top: 5px solid $color_green;
  border-radius: 20px 20px 0 0;
  border-bottom: 2px solid white;
}

img {
  width: 70%;
  height: auto;
}

#latestnews-bottom {
  width: 100%;
}
span {
  color: $color_green;
}
</style>
