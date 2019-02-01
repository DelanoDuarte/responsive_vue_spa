<template>
  <div>
    <about-me-component></about-me-component>
    <v-spacer></v-spacer>
    <skills-card-component></skills-card-component>
  </div>
</template>

<script>
import AboutMeComponent from "@/components/about/AboutMeComponent.vue";
import SkillsCardComponent from "@/components/about/SkillsCardComponent.vue";
export default {
  components: {
    AboutMeComponent,
    SkillsCardComponent
  }
};
</script>