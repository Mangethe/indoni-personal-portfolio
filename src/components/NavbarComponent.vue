<template>
    <header>
  <nav class="navbar is-dark is-fixed-top" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="index.html">
        <img src="../images/logo.png" width="112" height="28">
      </a>
  
      <a role="button" @click="handleClick" class="navbar-burger burger" aria-label="menu" aria-expanded="false" data-target="navigation" >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>
  
    <div id="navigation" class="navbar-menu">
      <div class="navbar-end">
        <a href="#index" class="navbar-item">Home</a>
        <a href="#about" class="navbar-item">About</a>
        <a href="blog.html" class="navbar-item">blog</a>
        <a href="/portfolio" class="navbar-item">portfolio</a>
        <a href="contact.html" class="navbar-item">contact</a>
      </div>
    </div>
  </nav>
</header>
</template>

<script>
// @ is an alias to /src
import $ from "jquery";
export default {
  name: "NavbarComponent",
  methods: {
    handleClick() {
      $(".filter-menu .button").click(function () {
		$(this).addClass("is-active").siblings().removeClass('is-active');
	});
    }
  }
};
</script>
