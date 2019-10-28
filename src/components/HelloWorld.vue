<template>
  <v-container>
    <v-layout
      text-center
      wrap
      fluid
    >
      <v-flex xs12>
        <v-img
          :src="require('../assets/logo_mario_kart.png')"
          class="my-3"
          contain
          height="200"
        ></v-img>
      </v-flex>

      <v-flex mb-4>
        <h1 class="display-1 font-weight-bold mb-3">
          Welcome to Mario Kart Competitions Stats
        </h1>    
      </v-flex>

      <v-flex
        xs12
        mb-5
      >
        <h2 class="headline font-weight-bold mb-3">Useful links</h2>

        <v-layout justify-center>
          <a
            v-for="(use, i) in usefullinks"
            :key="i"
            :href="use.href"
            class="subheading mx-3"
            target="_blank"
          >
            {{ use.text }}
          </a>
        </v-layout>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    usefullinks: [
      {
        text: 'GitHub',
        href: 'https://github.com/AntoninLatour/Repo',
      },
    ]
  }),
};
</script>
