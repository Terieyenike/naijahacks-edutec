<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-light py-3">
      <div class="container-fluid">
        <router-link class="navbar-brand logo" to="/">
          <strong>Edutec</strong>
          <span class="sr-only">(current)</span>
        </router-link>
        <button
          class="navbar-toggler"
          type="button"
          data-toggle="collapse"
          data-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav ml-auto">
            <li class="nav-item">
              <router-link class="nav-link" to="/about">About Us</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/careers">Careers</router-link>
            </li>

            <li class="nav-item">
              <router-link class="nav-link" to="/community">Community</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/faq">FAQ</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/contact">Contact us</router-link>
            </li>
            <li class="nav-item dropdown">
              <a
                class="nav-link dropdown-toggle"
                href="#"
                id="navbarDropdown"
                role="button"
                data-toggle="dropdown"
                aria-haspopup="true"
                aria-expanded="false"
              >Sign Up / Sign In</a>
              <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                <router-link class="dropdown-item" to="/signup">Sign Up</router-link>
                <router-link class="dropdown-item" to="/signin">Sign In</router-link>
              </div>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <router-view />
  </div>
</template>

<style lang="scss">
@import '@/assets/sass/_variables.scss';
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

li.nav-item {
  margin-right: 20px;
}
</style>
