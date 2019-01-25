<template>
  <div class="home">
    <v-container grid-list-md>
      <v-layout row wrap>
        <v-flex v-for="i in 3" :key="`4${i}`" xs4>
          <home-card-component></home-card-component>
        </v-flex>
      </v-layout>
    </v-container>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import HomeCardComponent from "@/components/home/HomeCardComponent.vue";

export default {
  name: "home",
  components: {
    HelloWorld,
    HomeCardComponent
  }
};
</script>
