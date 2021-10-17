<template>
  <v-card
    class="mx-auto"
    max-width="344"
     flat
    outlined
  >
    <v-card-text>
      <p class="text-h4 text--primary mt-2">
        Prediction
        </p>
        <v-divider></v-divider>

      <div class="text--primary">
        <PredictionList/>
      </div>
    </v-card-text>
    

  </v-card>
</template>

<script>
import PredictionList from './PredictionList'
export default{
    name:"PredictionCard",
    components:{PredictionList},
    data: () => ({
      reveal: false,
    }),
}
</script>
<style>
.v-card--reveal {
  bottom: 0;
  opacity: 1 !important;
  position: absolute;
  width: 100%;
}
</style>