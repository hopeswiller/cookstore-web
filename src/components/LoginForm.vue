<template>
  <form action="#" method="post" @submit.prevent>
    <div class="form-group first" style="text-align: left">
      <label for="username">Username</label>
      <input
        type="text"
        class="form-control"
        placeholder="Username"
        id="username"
      />
    </div>
    <div class="form-group last mb-3" style="text-align: left">
      <label for="password">Password</label>
      <input
        type="password"
        class="form-control"
        placeholder="Password"
        id="password"
      />
    </div>

    <div class="d-sm-flex mb-5 align-items-center">
      <label class="control control--checkbox mb-3 mb-sm-0"
        ><span class="caption">Remember me</span>
        <input type="checkbox" checked="checked" />
        <div class="control__indicator"></div>
      </label>
      <span class="ml-auto">
        <a href="#" class="forgot-pass">Forgot Password</a>
      </span>
    </div>
    <input
      type="submit"
      value="Log In"
      class="btn btn-block py-2 btn-primary"
    />

    <span class="text-center my-3 d-block"
      >or
      <hr
    /></span>

    <div class="">
      <a href="#" class="btn btn-block py-2 btn-facebook">
        <span class="icon-facebook mr-3"></span> Login with facebook
      </a>
      <a href="#" class="btn btn-block py-2 btn-google"
        ><span class="icon-google mr-3"></span> Login with Google</a
      >
    </div>
  </form>
</template>

<script>
export default {
  name: "LoginForm",
  data() {
    return {};
  },
};
</script>

<style scoped>
.forgot-pass {
  position: relative;
  top: 2px;
  font-size: 14px;
}

.form-control {
  border: none;
  border-radius: 4px;
  height: 54px;
  background: #efefef;
}
.form-control:active,
.form-control:focus {
  outline: none;
  -webkit-box-shadow: none;
  box-shadow: none;
}

.btn-facebook {
  display: block;
  background: #3b5998;
  color: #fff;
  text-decoration: none !important;
}
.btn-google {
  background: #ea4335;
  color: #fff;
  text-decoration: none !important;
}
</style>
