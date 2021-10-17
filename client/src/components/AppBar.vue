<template>
  <v-card class="overflow-hidden">
    <v-app-bar
      absolute
      color="#e82127"
      dark
      shrink-on-scroll
      prominent
      fade-img-on-scroll
      scroll-target="#scrolling-techniques-3"
    >
<v-app-bar-title class="ml-6">Battery Analysis</v-app-bar-title>


      <template v-slot:extension>
        <v-tabs align-with-title>
          <v-tab>Input Tests</v-tab>
          <v-tab>calculator</v-tab>
          <v-tab>Test Results</v-tab>
        </v-tabs>
      </template>
    </v-app-bar>
    <v-sheet
      id="scrolling-techniques-3"
      class="overflow-y-auto"
      max-height="600"
    >
      <v-container style="height: 1000px;"></v-container>
    </v-sheet>
  </v-card>
</template>
<script>


export default {
  name: 'AppBar',
  data(){
      return {
          
      }
  }



  
};
</script>
