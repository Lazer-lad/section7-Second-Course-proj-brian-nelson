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
        <v-row>
            <v-col cols="12">
                <header>
                    <h1>Server status
                    </h1>
                </header>
            </v-col>
        </v-row>
        <hr>
        <v-row>
            <v-col cols="6">
        
                <v-list>
                    <v-list-item-content v-for="index in 5" :key="index">
                      
                    Server #{{ index }}
<v-divider :inset="inset"></v-divider>

                    </v-list-item-content>
                </v-list>
            </v-col>
            <v-col cols="6">
                <p>Server Details are currently not updated</p>
            </v-col>
        </v-row>
        <hr>
        <v-row>
            <v-col cols="12">
                <footer>
                    <p>All Servers are managed here</p>
                </footer>
            </v-col>
        </v-row>
    </v-container>
  </v-app>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld';
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import servers from './components/Servers.vue';
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