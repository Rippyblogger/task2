<template>
  <v-app>
    <v-app-bar
      app
      color="primary"
      dark
    >
      <div class="d-flex align-center">

        <v-img
          alt="Vuetify Name"
          class="shrink mt-1 hidden-sm-and-down"
          contain
          min-width="50"
          src="../src/assets/4vHpZnpa_400x400.jpg"
          width="50"
        />
      </div>

      <v-spacer></v-spacer>

      
    </v-app-bar>

    <v-main>
      <HelloWorld/>
      <Jobcard/>
      <Skillcard class="spaceme"/>
    </v-main>
  </v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld';
import Jobcard from './components/Jobcard';
import Skillcard from './components/Skillcard';

export default {
  name: 'App',

  components: {
    HelloWorld,
    Jobcard,
    Skillcard,
  },

  data: () => ({
    //
  }),
};
</script>

<style>

.spaceme{
  margin-top: 1rem
}

</style>
