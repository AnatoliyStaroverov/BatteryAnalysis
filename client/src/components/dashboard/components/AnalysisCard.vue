<template>
  <v-card
    class="mx-auto"
    max-width="344"
    flat
    outlined

  >
    <v-card-text>
      <p class="text-h4 text--primary mt-2">
         Results
        </p>
        <v-divider></v-divider>

      <div class="text--primary">
        <AnalysisList/>
      </div>
    </v-card-text>
    

  </v-card>
</template>

<script>
import AnalysisList from './AnalysisList'
export default{
    name:"AnalysisCard",
    components:{AnalysisList},
    data: () => ({
      reveal: false,
    }),
}
</script>
<style>
.card{
    
}
</style>