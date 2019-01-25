<template>
  <div class="bottom_menu">
    <v-bottom-nav class="navbottom animated bounceInLeft" fixed color="dark">
      <v-btn color="teal" flat value="recent">
        <span>Home</span>
        <v-icon>fas fa-home</v-icon>
      </v-btn>

      <v-btn color="teal" flat value="favorites">
        <span>About Me</span>
        <v-icon>fas fa-user-circle</v-icon>
      </v-btn>

      <v-btn color="teal" flat value="nearby">
        <span>Location</span>
        <v-icon>fas fa-map-marker</v-icon>
      </v-btn>
    </v-bottom-nav>
  </div>
</template>

<script>
export default {
  name: "appfooter"
};
</script>

<style scoped>
.bottom_menu {
  display: none;
}

@media screen and (max-width: 700px) {
  .bottom_menu {
    display: flex;
  }
  .navbottom {
    display: flex;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: 1030;
    bottom: 0;
    height: auto !important;
  }
}
</style>
