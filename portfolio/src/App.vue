<template>
  <v-container fluid grid-list-md class="pt-0 px-0">
    <v-app>
      <v-row>
        <v-col cols="3">
          <side-bar></side-bar>
        </v-col>
        <v-col>
          <v-app-bar app color="white" dark>
            <v-btn outlined
              ><router-link :to="{ name: 'Home' }" class="text-decoration"
                >Home</router-link
              ></v-btn
            >
            <v-btn outlined class="mx-2"
              ><router-link :to="{ name: 'About' }" class="text-decoration"
                >About</router-link
              ></v-btn
            >
            <v-btn outlined>
              <router-link :to="{ name: 'Projects' }" class="text-decoration"
                >Projects</router-link
              ></v-btn
            >
            <v-btn outlined class="mx-2"
              ><router-link :to="{ name: 'Contacts' }" class="text-decoration"
                >Contact</router-link
              ></v-btn
            >
          </v-app-bar>
          <v-main>
            <v-card outlined :elevation="0" class="pa-6" height="788">
              <router-view />
            </v-card>
          </v-main>
        </v-col>
      </v-row>
    </v-app>
  </v-container>
</template>

<script>
import SideBar from "./components/SideBar.vue";
export default {
  name: "App",
  components: {
    SideBar,
  },
  data: () => ({
    //
  }),
};
</script>
<style scoped>
.text-decoration {
  text-decoration: none;
  color: wheat;
}
</style>
