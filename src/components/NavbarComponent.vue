<template>
  <nav class="navbar is-transparent is-fixed" role="navigation" aria-label="main navigation">
  <div class="navbar-brand">
    <a role="button" class="navbar-burger" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="navbarBasicExample" class="navbar-menu">
    <div class="navbar-end">
      <router-link to="/" class="navbar-item">
        Home
      </router-link>

      <router-link to="/services" class="navbar-item">
        Services
      </router-link>

      <router-link to="/projects" class="navbar-item">
        About
      </router-link>

      <router-link to="/about" class="navbar-item">
        About
      </router-link>

      <router-link to="/contact" class="navbar-item">
        Contact
      </router-link>
 
    </div>
  </div>
</nav>
</template>

<script>
// @ is an alias to /src

export default {
  name: "NavbarComponent"
};
</script>
