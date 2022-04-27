<template>
  <div class="sidebar-wrapper">
    <ul class="nav" id="nav">
      <li>
        <router-link to="/">
          <i class="nc-icon nc-bank"></i>
          <p>Home</p>
        </router-link>
      </li>
      <li>
        <router-link to="/table">
          <i class="nc-icon nc-tile-56"></i>
          <p>Table List</p>
        </router-link>
      </li>
      <li>
        <router-link to="/user">
          <i class="nc-icon nc-single-02"></i>
          <p>User Profile</p>
        </router-link>
      </li>
      <li>
        <router-link to="/typo">
          <i class="nc-icon nc-caps-small"></i>
          <p>Typography</p>
        </router-link>
      </li>
    </ul>
  </div>
</template>

<style scoped>
#nav a.router-link-exact-active {
  color: #ef8157;
  opacity: 1;
}
</style>
