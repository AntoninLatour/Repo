<template>
  <v-app>
    <v-app-bar app dark color="red darken-2">
      <v-toolbar-title class="headline text-uppercase">
        <span>MARIO KART</span>
        <span class="font-weight-light"> COMPETITON</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>
        <span class="mr-2">Dev version</span>
    </v-app-bar>

    <v-content>
      <Login/>
    </v-content>
  </v-app>
</template>

<script>
import Login from './components/Login';

export default {
  name: 'App',
  components: {
    Login,
  },
  data: () => ({
    //
  }),
};
</script>
