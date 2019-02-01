<template>
  <div class="home animated fadeIn">
    <v-card>
      <v-container fluid grid-list-lg>
        <v-layout row wrap>
          <v-flex>
            <!-- v-for="i in 3" :key="`4${i}`" -->
            <home-card-component></home-card-component>
          </v-flex>
          <v-flex>
            <!-- v-for="i in 3" :key="`4${i}`" -->
            <home-card-component></home-card-component>
          </v-flex>
          <v-flex>
            <!-- v-for="i in 3" :key="`4${i}`" -->
            <home-card-component></home-card-component>
          </v-flex>
        </v-layout>
      </v-container>
    </v-card>
  </div>
</template>

<script>
// @ is an alias to /src
import HomeCardComponent from "@/components/home/HomeCardComponent.vue";

export default {
  name: "home",
  components: {
    HomeCardComponent
  }
};
</script>
