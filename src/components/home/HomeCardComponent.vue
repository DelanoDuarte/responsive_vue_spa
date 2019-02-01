<template>
  <v-card class="animated bounceInRigth" color="cyan darken-2" dark style="max-width: 400px;">
    <v-layout align-center justify-center fill-height>
      <v-flex xs8>
        <v-card-title primary-title>
          <div>
            <div class="headline">Halycon Days</div>
            <div>Ellie Goulding</div>
            <div>(2013)</div>
          </div>
        </v-card-title>
      </v-flex>
      <v-img
        class="shrink ma-2"
        contain
        height="125px"
        src="https://cdn.vuetifyjs.com/images/cards/halcyon.png"
        style="flex-basis: 125px"
      ></v-img>
    </v-layout>
    <v-divider dark></v-divider>
    <v-card-actions class="pa-3">Rate this album
      <v-spacer></v-spacer>
      <span class="grey--text text--lighten-2 caption mr-2">({{ formatRatingText(rating) }})</span>
      <v-rating
        v-model="rating"
        background-color="white"
        color="yellow accent-4"
        dense
        hover
        size="18"
      ></v-rating>
    </v-card-actions>
  </v-card>
</template>

<script>
export default {
  name: "",
  data() {
    return {
      rating: 0
    };
  },
  methods: {
    formatRatingText(rating) {
      return `${rating} - ${this.returnTextTypeBasedOnRating(rating)}`;
    },

    returnTextTypeBasedOnRating(rating) {
      switch (rating) {
        case 0 && rating < 1:
          return "Urrrgh !!";

        case 1 || (rating < 2 && rating > 1):
          return "Try again next time ...";

        case 2 || (rating < 3 && rating > 2):
          return "Could be better.";

        case 3 || (rating < 4 && rating > 3):
          return "OK !!";

        case 4 || (rating < 5 && rating > 4):
          return "Nice, I like it ...";

        case 5:
          return "Yeaah Baby,Awesome !";
      }
    }
  }
};
</script>

<style>
</style>
