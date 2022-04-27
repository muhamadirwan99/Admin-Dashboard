<template>
  <div class="wrapper">
    <div class="sidebar" data-color="white" data-active-color="danger">
      <div class="logo">
        <a href="https://www.creative-tim.com" class="simple-text logo-mini">
          <div class="logo-image-small">
            <img src="assets/img/logo-small.png" />
          </div>
        </a>
        <a href="https://www.creative-tim.com" class="simple-text logo-normal">
          Menu
          <!-- <div class="logo-image-big">
            <img src="assets/img/logo-big.png" />
          </div> -->
        </a>
      </div>
      <!-- Sidebar -->
      <SidebarComp />
    </div>
    <div class="main-panel">
      <!-- Navigation -->
      <NavComp />
      <!-- Main Content -->
      <router-view />
      <!-- Footer -->
      <FooterComp />
    </div>
  </div>
</template>

<script>
// Components
import FooterComp from "./components/FooterComp.vue";
import NavComp from "./components/NavComp.vue";
import SidebarComp from "./components/SidebarComp.vue";

export default {
  name: "App",
  components: {
    FooterComp,
    NavComp,
    SidebarComp,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
