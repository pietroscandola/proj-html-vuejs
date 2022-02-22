<template>
  <section class="bg-image">
    <div class="container">
      <h2 class="text-center">Sign up to our Newsletter</h2>

      <div class="input py-2">
        <input type="text" name="newsletter" v-model="email" />
        <div v-if="succesMail" class="alert text-center" role="alert">
          Email inviata correttamente
        </div>
      </div>
      <div class="py-3">
        <button class="button text-center w-100" @click="checkMail">
          SUBSCRIVE
        </button>
      </div>

      <p class="text-center">
        (We do not share your data with anybody, and only use it for its
        intended purpose)
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "Newsletter",
  data() {
    return {
      email: "",
      succesMail: false,
    };
  },
  methods: {
    checkMail() {
      if (!this.email) return;
      this.succesMail = true;
      this.email = "";
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../../assets/scss/style.scss";
.container {
  width: 30%;
}

.bg-image {
  background-image: url("../../assets/img/newsletter_background.jpg");
  min-width: 100%;
  height: 350px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}

h2 {
  padding-top: 50px;
  padding-bottom: 30px;
}
p {
  color: $color_gray;
  font-size: 14px;
}
input {
  width: 100%;
  padding: 10px;
}
.input {
  position: relative;
}

.alert {
  position: absolute;
  top: 4px;
}
</style>
