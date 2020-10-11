<template>
  <div class="home">
    <Figma :figma="figmaConfig" v-model="viewModel" />
  </div>
</template>

<script>
import Vue from "vue";
import Figma from "vue-low-code";
Vue.use(Figma);

// import JSON file for deployment
import app from "./app.json";

export default {
  name: "Home",
  data: function() {
    return {
      figmaJSON: app,
      figmaConfig: {
        figmaFile: "ine8bnxFRsTfxskewHSAv8",
        figmaAccessKey: "68678-d96bffc3-79a4-4ea2-89d6-47ef2c7f48ac",
      },
      viewModel: {
        /**
         * Add your view model here
         */
      },
      config: {
        components: {
          /**
           * Register costum components here
           */
        },
      },
    };
  },
  components: {},
  methods: {
    /**
     * Place your methods here
     */
  },
};
</script>
