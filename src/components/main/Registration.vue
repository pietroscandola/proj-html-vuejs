<template>
  <section>
    <div class="container">
      <div class="row">
        <div class="col-6">
          <h2 id="title" class="pt-5">Get Behind the Wheel</h2>
          <p class="py-3 fs-5 text">
            Lorem ipsum dolor, sit amet consectetur adipisicing elit. Magni,
            ipsam. Amet, fuga. Accusamus tempora tenetur similique unde odit
            ducimus voluptate vel atque eligendi suscipit, necessitatibus ex
            laudantium, impedit corporis. Omnis!
          </p>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Non tenetur
            ipsam debitis blanditiis pariatur culpa necessitatibus modi, vitae
            voluptatem voluptatibus amet consequatur ipsa dicta doloremque
            ratione excepturi? Illo, odio aspernatur!
          </p>
        </div>
        <div class="col-6">
          <div class="card p-3">
            <h2 id="lesson" class="text-center py-2">First Lesson Free</h2>
            <p class="text-center py-2">
              When you make a block booking with us your first lesson is
              included free.
            </p>

            <div class="input-group my-3">
              <input
                type="text"
                class="form-control py-2"
                placeholder="Your Name*"
                v-model="name"
              />
              <span class="input-group-text"
                ><img src="../../assets/img/image.png" alt="image"
              /></span>
            </div>
            <div class="input-group my-3">
              <input
                type="text"
                class="form-control py-2"
                placeholder="Email*"
                required
                v-model="email"
              />
            </div>
            <div class="input-group my-3">
              <input
                type="tel"
                class="form-control py-2"
                placeholder="Telephone"
                v-model="phone"
                @input="acceptNumber"
              />
            </div>
            <div class="input-group my-3">
              <input
                type="text"
                class="form-control py-2"
                placeholder="Location"
                v-model="location"
              />
            </div>
            <div class="text-center my-3">
              <button class="w-50 button" @click="requestCall">
                REQUEST A CALLBACK
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Registration",
  data() {
    return {
      name: "",
      email: "",
      phone: "",
      location: "",
    };
  },
  watch: {
    email(value) {
      this.email = value;
      this.validateEmail(value);
    },
  },
  methods: {
    acceptNumber() {
      const n = this.phone
        .replace(/\D/g, "")
        .match(/(\d{0,3})(\d{0,3})(\d{0,4})/);
      this.phone = !n[2] ? n[1] : "" + n[1] + " " + n[2] + (n[3] ? +n[3] : "");
    },

    validateEmail(value) {
      if (/^\w+([.-]?\w+)*@\w+([.-]?\w+)*(\.\w{2,3})+$/.test(value)) {
        this.msg["email"] = "";
      } else {
        this.msg["email"] = "Please enter a valid email address";
      }
    },

    requestCall() {
      this.name = "";
      this.email = "";
      this.phone = "";
      this.location = "";
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";
.row {
  margin: 60px 0 150px 0;
}

#title {
  font-size: 3rem;
}

input {
  border-right: 0;
}

.input-group-text {
  background-color: white;
  border-left: 0;
}
.card {
  width: 30%;
  border-radius: 30px;
  position: absolute;
  margin-top: -90px;
}
button {
  border-radius: 20px;
  padding: 10px;
  color: white;
  font-weight: 400;
  background-color: $color_green;
}

#lesson {
  color: $color_green;
}
</style>
