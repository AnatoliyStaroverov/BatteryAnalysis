<template>
  <v-app >
   <v-card  color="#e82127">
    <v-card-title class="text-center justify-center py-6">
      <h1 class="font-weight-bold text-h3 header-text ">
        Battery Analysis
      </h1>
    </v-card-title>
    <v-tabs 
       background-color="#C9CBCC"
       color="#e82127"
         grow
    >
    <v-tab href="#dash-board">
         Home
      </v-tab>
      <v-tab-item class="main" value="dash-board">
        <DashBoard/>
      </v-tab-item>

      <v-tab href="#test-input">
         Test Inputs
      </v-tab>
      <v-tab-item class="main" value="test-input">
        <TestInputs/>
      </v-tab-item>
      <v-tab href="#test-results">
         Test Results
      </v-tab>
      <v-tab-item class="main" value="test-results">
        <TestResults/>
      </v-tab-item>
      <v-tab href="#test-predictions">
          Test Predictions
      </v-tab>
      <v-tab-item class="main" value="test-predictions">
        <TestPredictions/>
      </v-tab-item>
    </v-tabs>
  </v-card>
 </v-app>
</template>
<script>

import TestInputs from './components/test-inputs/views/TestInputs'
import TestResults from './components/test-results/views/TestResults'
import TestPredictions from './components/test-predictions/views/TestPredictions'
import DashBoard from './components/dashboard/views/DashBoard'

export default {
  name: 'App',
  components:{
    TestInputs,
    TestResults,
    TestPredictions,
    DashBoard
  },

};
</script>
<style>


.main{

  height:100%;
}
.header {
  background-color: #e82127 !important;
}
.header-text  {
  color: white !important;
}
</style>
