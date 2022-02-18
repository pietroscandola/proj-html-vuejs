<template>
  <section>
    <div class="bg-image">
      <div class="container">
        <div class="row py-5">
          <div class="col-6 d-flex align-items-center">
            <div>
              <h2 class="text-white">Start Learning to Drive Today</h2>
              <p class="text-white">
                Give us a call to schedule your first driving lesson
              </p>
            </div>
          </div>
          <div class="col-6 d-flex justify-content-center align-items-center">
            <i class="fa-solid fa-phone-flip px-5 text-white"></i>
            <span class="text-white">1-800-555-555</span>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Phone",
};
</script>

<style lang="scss" scoped>
.bg-image {
  background-image: url("../../assets/img/horizontal-cta-background.jpg");
  min-width: 100%;
  min-height: 200px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
h2 {
  font-size: 2.5rem;
}

p {
  font-size: 1.2rem;
  font-weight: 500;
}

span {
  font-size: 2.5rem;
}
i {
  font-size: 3rem;
}
</style>
