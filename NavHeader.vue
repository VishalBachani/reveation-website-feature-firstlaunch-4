<template>
  <b-navbar fixed="top" toggleable="lg" type="dark" class="px-5 py-3 rl-header" v-bind:class="{ 'rl-header-scrolled': addHeaderBackground }">
    <b-container fluid class="nav-menu-container">
      <!-- //TODO: header needs more work -->  
      <b-navbar-brand tag="h1">Reveation Labs</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
      <b-collapse id="nav-collapse" is-nav>        
        <b-navbar-nav class="ml-auto">
          <b-nav-item href="#">Home</b-nav-item>
          <b-nav-item v-scroll-to="{ el: '#about', offset: -72 }" href="#">About Us</b-nav-item> 
          <b-nav-item v-scroll-to="{ el: '#services', offset: -72 }" href="#">Services</b-nav-item>
          <!--
          <b-nav-item-dropdown v-scroll-to="{ el: '#services', offset: -72 }" text="Services" right>
            <b-dropdown-item href="#">Moiblity Solutions</b-dropdown-item>
            <b-dropdown-item href="#">Digital Solutions</b-dropdown-item>
            <b-dropdown-item href="#">Cloud Solutions</b-dropdown-item>
            <b-dropdown-item href="#">XYZ Solutions</b-dropdown-item>
          </b-nav-item-dropdown>         
          -->
          <!-- <b-nav-item href="#">Portfolio</b-nav-item>  -->
          <b-nav-item href="#">Contact Us</b-nav-item>          
        </b-navbar-nav>
      </b-collapse>
    </b-container>
  </b-navbar>
</template>

<script>
import debounce from 'lodash/debounce';

export default {
  data() {
    return {
      addHeaderBackground: false
    };
  },
  methods: {
    handleScroll(event) {
      // Any code to be executed when the window is scrolled
      this.addHeaderBackground = (window.scrollY > 70);    
    }
  },
  created() {
    this.handleDebouncedScroll = debounce(this.handleScroll, 50);
    window.addEventListener('scroll', this.handleDebouncedScroll);
  },
  beforeDestroy() {
    // I switched the example from `destroyed` to `beforeDestroy`
    // to exercise your mind a bit. This lifecycle method works too.
    window.removeEventListener('scroll', this.handleDebouncedScroll);
  }
};
</script>

<style>
.nav-menu-container .nav-item {
  margin-left: 10px
}
.nav-menu-container .nav-item .nav-link {
  padding: 0 8px 10px;
  text-decoration: none;
  display: inline-block;
  color: #fff;
  font-family: montserrat,sans-serif;
  font-weight: 700;
  font-size: 13px;
  text-transform: uppercase;
  outline: none;
}
.nav-menu-container .nav-item:hover>.nav-link, .nav-menu-container .active>.nav-link {
  color: #18d26e;
}
.rl-header {
  height: 90px;
}
.rl-header-scrolled {
  background: rgba(0,0,0,.9);
  padding: 20px 0;
  height: 72px;
  transition: all .5s;
}
</style>