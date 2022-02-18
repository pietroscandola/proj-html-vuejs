<template>
  <div class="bg-image">
    <div class="container">
      <div class="row">
        <!-- Informazioni del Corso -->
        <div class="col-4">
          <div class="card-course p-5">
            <div id="new">NEW</div>
            <h2 class="text-center">Courses</h2>
            <p class="py-3">
              Lorem, ipsum dolor sit amet consectetur adipisicing elit. Vel in
              assumenda fugiat, ipsam quae rem aperiam deserunt modi tenetur? At
              quo expedita fuga consequatur dignissimos optio neque ad
              perspiciatis facilis?
            </p>
            <div class="text-center">
              <button class="button">Course Information</button>
            </div>
          </div>
        </div>

        <!-- Tipologie di Corso -->
        <div class="col-8">
          <div class="row">
            <div class="col-4">
              <div class="card">
                <img
                  src="../../assets/img/courses-passplus.jpg"
                  alt="Pass Plus Course"
                />
                <h5 class="text-center">Pass Plus</h5>
                <button class="button-outline py-2">Learn More</button>
              </div>
            </div>
            <div class="col-4">
              <div class="card">
                <img
                  src="../../assets/img/course-intensive.jpg"
                  alt="Intensive Course"
                />
                <h5 class="text-center">Pass Plus</h5>
                <button class="button-outline py-2">Learn More</button>
              </div>
            </div>
            <div class="col-4">
              <div class="card">
                <img
                  src="../../assets/img/courses-instructor.jpg"
                  alt="Instructors"
                />
                <h5 class="text-center">Intensive Course</h5>
                <button class="button-outline py-2">Learn more</button>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Course",
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";
.bg-image {
  background-image: url("../../assets/img/promise-background.jpg");
  min-width: 100%;
  min-height: 500px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

h2 {
  font-size: 3rem;
}
p {
  margin: 0 auto;
}

#new {
  background-color: $color_green;
  height: 60px;
  width: 80px;
  display: flex;
  justify-content: center;
  align-items: end;
  font-weight: 400;
  color: white;
  position: absolute;
  transform: rotate(-45deg);
  top: -22px;
  left: -33px;
}

.card-course {
  border: 3px solid $color_green;
  border-radius: 20px;
  position: absolute;
  margin-top: -30px;
  width: 20%;
  background-color: white;
  overflow: hidden;
}

.card {
  border: transparent;
  background-color: transparent;
}

img {
  padding: 30px;
}

.button-outline {
  margin: 0 50px;
}
</style>
