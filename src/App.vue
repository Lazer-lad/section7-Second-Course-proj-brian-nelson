<!--<template>
  

<div id="app">
  <v-app id="">
    <div>
      <div class="
         ">
        <v-card
          v-for="n in 3"
          :key="n"
          class="pa-2"
          outlined
          tile
        >
          Flex item {{ n }}
        </v-card>
      </div>
      <div class="d-flex flex-column-reverse">
        <v-card
          v-for="n in 3"
          :key="n"
          class="pa-2"
          outlined
          tile
        >
          Flex item {{ n }}
        </v-card>
      </div>
    </div>
  </v-app>
</div>

</template>-->


<template>
<div id="app">
  <v-app id="test">
    <v-container>
<app-header></app-header>
      <hr>
        <v-row>
            <app-servers></app-servers>
            <app-server-details></app-server-details>
        </v-row>
        <hr>
        <app-footer></app-footer>
    </v-container>
  </v-app>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld';
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Servers from './components/Servers.vue';
import ServerDetails from './components/ServerDetails.vue';

export default {
  name: 'App',
  components: {
    //HelloWorld,
    'app-header': Header,
    'app-footer': Footer,
    'app-servers': Servers,
    'app-server-details': ServerDetails,
  },
  data: () => ({
    //
  }),
};
</script>