<template>
  <div class="bottom_menu">
    <v-bottom-nav class="navbottom animated bounceInLeft" fixed color="dark" :active.sync="path">
      <v-btn color="teal" flat value="/" @click="goTo('/')">
        <span>Home</span>
        <v-icon>fas fa-home</v-icon>
      </v-btn>

      <v-btn color="teal" flat value="/about" @click="goTo('/about')">
        <span>About Me</span>
        <v-icon>fas fa-user-circle</v-icon>
      </v-btn>

      <v-btn color="teal" flat value="/location">
        <span>Location</span>
        <v-icon>fas fa-map-marker</v-icon>
      </v-btn>
    </v-bottom-nav>
  </div>
</template>

<script>
export default {
  name: "appfooter",
  data() {
    return {
      path: window.location.pathname
    };
  },
  methods: {
    goTo(link) {
      this.$router.push(link);
    }
  }
};
</script>

<style scoped>
.bottom_menu {
  display: none;
  padding-top: 50px;
}

@media screen and (max-width: 700px) {
  .bottom_menu {
    display: flex;
  }
  .navbottom {
    display: flex;
    position: fixed;
    right: 0;
    bottom: 0;
    left: 0;
    z-index: 1030;
    bottom: 0;
    height: auto !important;
  }
}
</style>
