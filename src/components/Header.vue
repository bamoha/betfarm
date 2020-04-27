<template>
  <div class="main-nav">
    <b-navbar toggleable="lg" type="light">
      <div target="nav-collapse">
        <img src="../assets/menu.svg" alt />
        <span class="nav-text ml-2">A-Z</span>
      </div>

      <b-navbar-brand href="#">
        <img height="34" width="103" src="../assets/betfarmlogo.png" alt />
      </b-navbar-brand>

      <img src="../assets/Vector.svg" alt />

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">Link</b-nav-item>
          <b-nav-item href="#" disabled>Disabled</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template v-slot:button-content>
              <em>User</em>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <div class="d-flex justify-content-between px-3">
        <b-button class="nav-btn register">JOIN NOW</b-button>
        <b-button class="nav-btn login">LOGIN</b-button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
};
</script>