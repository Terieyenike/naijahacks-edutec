<template>
  <div class="container space-top pb-5">
    <div class="row">
      <div class="col-lg-4 col-md-4 col-sm-12 mx-md-auto mb-md-4">
        <div>
          <img
            src="../../assets/images/undraw_Hello_qnas.svg"
            alt="illustration of a person welcoming"
            class="img-fluid"
          />
        </div>
      </div>
      <div class="col-lg-7 ml-auto col-sm-12">
        <div class="mb-3">
          <button type="button" class="btn btn-lg btn-block google-login">Sign up with Google</button>
        </div>
        <div class="mb-3">
          <button type="button" class="btn btn-lg btn-block facebook-login">Sign up with Facebook</button>
        </div>
        <form action @submit.prevent class="pt-4">
          <h2 class="text-green">Sign Up For An Account</h2>
          <p>Gain access to an endless collection of knowledge at the push of a button</p>
          <div class="row">
            <div class="col-sm-12 col-md-6 mb-3">
              <input
                type="text"
                class="form-control"
                id="firtsname"
                name="firstname"
                placeholder="First Name"
              />
            </div>
            <div class="col-sm-12 col-md-6 mb-3">
              <input
                type="text"
                class="form-control"
                id="lastname"
                name="lastname"
                placeholder="Last Name"
              />
            </div>
          </div>
          <div class="row">
            <div class="col-sm-12 col-md-6 mb-3">
              <input
                type="email"
                class="form-control"
                id="email"
                name="email"
                placeholder="Email Adress"
              />
            </div>
            <div class="col-sm-12 col-md-6 mb-3">
              <input
                type="number"
                class="form-control"
                id="phoneNumber"
                name="phonerNumber"
                placeholder="Phone Number"
              />
            </div>
          </div>
          <div class="form-group">
            <input
              class="form-control"
              type="password"
              name="password"
              id="password"
              placeholder="Password"
            />
          </div>
          <div class="form-group">
            <input
              class="form-control"
              type="password"
              name="passwordAgain"
              id="passwordAgain"
              placeholder="Verify Password"
            />
          </div>
          <div class="row">
            <div class="col-sm-12">
              <p class="text-center">
                By clicking Create Account, you agree
                <a href="#">Terms of Use</a> and
                <a href="#">Privacy Policy</a>
              </p>
            </div>
          </div>
          <div class="form-group">
            <button type="submit" class="btn btn-lg btn-block form-action-button">Create Account</button>
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '@/assets/sass/_variables.scss';

.form-action-button {
  background: $dark-green;
  color: $white;
  padding-top: 1rem;
  padding-bottom: 1rem;

  &:hover {
    background: lighten($color: $dark-green, $amount: 4);
    color: $white;
    transition: background 0.3s;
  }
}
</style>