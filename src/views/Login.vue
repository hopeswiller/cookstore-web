<template>
  <div class="login">
    <div class="d-md-flex">
      <div class="bg" style="background-image: url('img/login_bg.jpg');"></div>
      
      <!-- <div class="bg" style="background-image: url('../src/assets/login_bg.jpg');"></div> -->
      
      <div class="contents">
        <div class="container">
          <div class="row align-items-center justify-content-center">
            <div class="col-md-12">
              <div class="form-block mx-auto">
                <div class="text-center mb-5">
                  <h3 class="text-uppercase">
                    Login to <strong>Cookstore</strong>
                  </h3>
                </div>
                <LoginForm />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import LoginForm from "@/components/LoginForm.vue";

export default {
  name: "Login",
  components: {
    LoginForm,
  },
};
</script>

<style scoped>
.container > .row {
  height: 100vh;
  min-height: 700px;
}

.contents {
  background: #f6f7fc;
  width: 75%;
}

.bg {
  width: 25%;
  background-size: cover;
  background-position: center;
}
@media (max-width: 767.98px) {
  .bg {
    width: 100%;
    height: 200px;
  }
  .contents {
    width: 100%;
  }
  .form-block {
    padding: 25px;
  }
}

.form-block {
  background: #fff;
  padding: 40px;
  max-width: 500px;
  -webkit-box-shadow: 0 15px 30px 0 rgba(0, 0, 0, 0.5);
  box-shadow: 0 15px 30px 0 rgba(0, 0, 0, 0.2);
}

a {
  color: #888;
  text-decoration: underline;
}


</style>
