<template>
  <v-layout justify-center>
    <v-flex xs12 sm6>
      <v-card>
        <v-container fluid grid-list-md>
          <v-layout row wrap>
            <v-flex v-for="card in cards" v-bind="{ [`xs${card.flex}`]: true }" :key="card.title">
              <v-card>
                <v-img :src="card.src" height="200px">
                  <v-container fill-height fluid pa-2>
                    <v-layout fill-height>
                      <v-flex xs12 align-end flexbox>
                        <span class="headline white--text" v-text="card.title"></span>
                      </v-flex>
                    </v-layout>
                  </v-container>
                </v-img>

                <v-card-actions>
                  <v-spacer></v-spacer>
                  <v-btn icon>
                    <v-icon>fas fa-heart</v-icon>
                  </v-btn>
                  <v-btn icon>
                    <v-icon>fas fa-bookmark</v-icon>
                  </v-btn>
                  <v-btn icon>
                    <v-icon>fas fa-share</v-icon>
                  </v-btn>
                </v-card-actions>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  data() {
    return {
      cards: [
        {
          title: "Pre-fab homes",
          src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
          flex: 12
        },
        {
          title: "Favorite road trips",
          src: "https://cdn.vuetifyjs.com/images/cards/road.jpg",
          flex: 6
        },
        {
          title: "Best airlines",
          src: "https://cdn.vuetifyjs.com/images/cards/plane.jpg",
          flex: 6
        }
      ]
    };
  }
};
</script>

<style>
</style>
