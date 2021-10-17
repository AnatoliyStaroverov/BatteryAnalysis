<template>
  <v-card
    class="mx-auto"
    max-width="344"
    flat
    outlined
  >
    <v-card-text>
      <p class="text-h4 text--primary mt-2">
        <v-badge color="#e82127"
          content="new"
        >
          Tests
        </v-badge>
        </p>
        <v-divider></v-divider>

      <div class="text--primary">
        <TotaltestList/>
      </div>
    </v-card-text>
    <v-card-actions class="mt-8">
      <v-btn
        text
        color="#e82127"
        @click="reveal = true"
      >
        Learn More
      </v-btn>
    </v-card-actions>

    <v-expand-transition>
      <v-card
        v-if="reveal"
        class="transition-fast-in-fast-out v-card--reveal"
        style="height: 100%;"
      >
        <v-card-text class="pb-0">
          <p class="text-h4 text--primary">
            Origin
          </p>
          <p>late 16th century (as a noun denoting a place where alms were distributed): from medieval Latin eleemosynarius, from late Latin eleemosyna ‘alms’, from Greek eleēmosunē ‘compassion’ </p>
        </v-card-text>
        <v-card-actions class="pt-0">
          <v-btn
            text
            color="#e82127"
            @click="reveal = false"
          >
            Close
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-expand-transition>
  </v-card>
</template>

<script>

import TotaltestList from './TotalTestList'
export default{
    name:"TotalTestsCard",
    components:{
        TotaltestList
        },
        
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