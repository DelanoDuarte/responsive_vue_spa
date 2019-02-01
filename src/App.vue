<template>
  <div id="app">
    <nav-bar></nav-bar>
    <section>
      <!-- <div id="nav" class="animated fadeIn">
        <router-link to="/">Home</router-link>|
        <router-link to="/about">About</router-link>
      </div>-->
      <router-view/>
    </section>

    <footer>
      <appfooter></appfooter>
    </footer>
  </div>
</template>

<script>
import NavBar from "@/components/layout/NavBar.vue";
import Footer from "@/components/layout/Footer.vue";
export default {
  components: {
    NavBar,
    appfooter: Footer
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}

section {
  padding-top: 10px;
}
</style>
