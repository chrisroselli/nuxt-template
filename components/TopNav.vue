<template>
    <b-navbar toggleable="lg" type="dark" variant="secondary" sticky>
    <b-navbar-brand href="#"><b-img src="logo.png" fluid alt="Responsive image"></b-img></b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>
<!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="/">Home</b-nav-item>
        <b-nav-item href="/about-us">About Us</b-nav-item>
        <b-nav-item href="/services">Services</b-nav-item>
        <b-nav-item href="/contact-us">Contact Us</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>
