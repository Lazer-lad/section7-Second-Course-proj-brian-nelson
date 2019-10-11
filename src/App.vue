<template>
  <div id="app">
    <v-app id="test">
      <v-container>
        <app-header></app-header>
        <hr />
        <v-row>
          <app-servers></app-servers>
          <app-server-details></app-server-details>
        </v-row>
        <hr />
        <app-footer></app-footer>
      </v-container>
    </v-app>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld';
import Header from "./components/Header.vue";
import Footer from "./components/Footer.vue";
import Servers from "./components/Servers.vue";
import ServerDetails from "./components/ServerDetails.vue";

export default {
  name: "App",
  components: {
    //HelloWorld,
    "app-header": Header,
    "app-footer": Footer,
    "app-servers": Servers,
    "app-server-details": ServerDetails
  },
  data: () => ({
    //
  })
};
</script>