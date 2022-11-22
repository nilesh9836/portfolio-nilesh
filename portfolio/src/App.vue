<template>
  <v-app>
    <v-main>
      <Home />
      <About />
    </v-main>
  </v-app>
</template>

<script>
import Home from "./components/Home";
import About from "./components/About";

export default {
  name: "App",

  components: {
    Home,
    About
  },

  data: () => ({
    //
  }),
};
</script>
