<template>
  <v-container fluid grid-list-lg>
    <v-layout row wrap>
      <v-flex xs12>
        <v-card color="cyan darken-2" class="white--text">
          <v-layout>
            <v-flex xs5>
              <v-img src="https://cdn.vuetifyjs.com/images/cards/foster.jpg" height="125px" contain></v-img>
            </v-flex>
            <v-flex xs7>
              <v-card-title primary-title>
                <div>
                  <div class="headline">Delano Junior</div>
                  <div>Fullstack Developer</div>
                  <!-- <div>(2014)</div> -->
                </div>
              </v-card-title>
            </v-flex>
          </v-layout>
          <v-divider light></v-divider>
          <v-card-actions class="pa-3">
            <v-layout row>
              <v-spacer></v-spacer>
              <div class="text-xs-center">
                <v-chip>
                  <v-avatar class="purple">J</v-avatar>Javascript
                </v-chip>
                <v-chip>
                  <v-avatar class="purple">J</v-avatar>Java
                </v-chip>
                <v-chip>
                  <v-avatar class="purple">P</v-avatar>Python
                </v-chip>
              </div>
            </v-layout>
          </v-card-actions>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {};
</script>

<style>
</style>
