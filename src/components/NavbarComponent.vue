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
        <div @click="handleNav('#parallax')" class="navbar-item pointer">Home</div>
        <div @click="handleNav('#About')" class="navbar-item pointer">About</div>
        <div @click="handleNav('#Blog')" class="navbar-item pointer">blog</div>
        <div @click="handleNav('#Portfolio')" class="navbar-item pointer">portfolio</div>
        <div @click="handleNav('#Contact')" class="navbar-item pointer">contact</div>
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
    },
    handleNav(navId) {
      console.log("HERE: ", navId);
      this.scrollTo(navId);

    },
    scrollTo(id) {
      $("html,body").animate({
        scrollTop: $(id).offset().top
      }, 2000);
    }
  }
};
</script>
