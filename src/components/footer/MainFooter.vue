<template>
  <section class="bg-image">
    <div class="container h-100">
      <div class="row h-100">
        <div class="col-3">
          <img
            src="../../assets/img/avada-drivers-logo-1x.png"
            alt="Logo Avada"
            class="py-3"
          />
          <p>
            Avada Driving School is the right choice for experienced drivers
            looking for a refrescher course, or the brand new driver wanting to
            pass first time
          </p>
        </div>
        <div class="col-3">
          <h4 class="py-3">CONTACT DETAILS</h4>
          <ul class="contacts">
            <li class="py-2">
              <i class="fa-solid fa-house-chimney pe-3"></i>
              <span>12345 North Main Street, New York, NY 555555</span>
            </li>
            <li class="py-2">
              <i class="fa-solid fa-phone-flip pe-3"></i>
              <span>1.800.555.6789</span>
            </li>
            <li class="py-2">
              <i class="fa-solid fa-envelope pe-3"></i>
              <span>info@your-domain.com</span>
            </li>
            <li class="py-2">
              <i class="fa-solid fa-link pe-3"></i>
              <span>Theme-Fusion</span>
            </li>
          </ul>
        </div>
        <div class="col-3">
          <h4 class="py-3">CONTACT DETAILS</h4>
          <ul>
            <li class="py-2">
              <i class="fa-solid fa-circle-arrow-right pe-3"></i
              ><span class="contact-details">Pass Plus</span>
            </li>
            <li class="py-2">
              <i class="fa-solid fa-circle-arrow-right pe-3"></i
              ><span class="contact-details">Intensive Course</span>
            </li>
            <li class="py-2">
              <i class="fa-solid fa-circle-arrow-right pe-3"></i
              ><span class="contact-details">Automatic</span>
            </li>
            <li class="py-2">
              <i class="fa-solid fa-circle-arrow-right pe-3"></i
              ><span class="contact-details">Instructor Training</span>
            </li>
          </ul>
        </div>
        <div class="col-3">
          <figure class="d-flex justify-content-end">
            <img
              src="../../assets/img/footer-ad-grid.png"
              class="img-fluid"
              alt="img_footer"
            />
          </figure>
          <div class="d-flex justify-content-center">
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
@import "../../assets/scss/style.scss";
.bg-image {
  background-image: url("../../assets/img/footer-background-color.jpg");
  min-width: 100%;
  height: 450px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.row {
  padding: 70px;
}

li {
  list-style-type: none;
}
h4 {
  color: white;
}
.fa-circle-arrow-right,
.contact-details {
  color: $color_green;
}

.contacts,
p {
  color: $color_gray;
}
</style>
