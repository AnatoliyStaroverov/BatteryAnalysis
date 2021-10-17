<template>
<v-container>
    <v-row class="mb-15 mt-10">
        <v-col>
            <TotalTestsCard />
        </v-col>
        <v-col>
            <AnalysisCard  />
        </v-col>
        <v-col>
            <PredictionCard  />
        </v-col>
    </v-row>
</v-container>
</template>

<script>
import TotalTestsCard from '../components/TotalTestsCard'
import AnalysisCard from '../components/AnalysisCard'
import PredictionCard from '../components/PredictionCard'
export default{
    name:"DashBoard",
    components:{ 
        TotalTestsCard,
        AnalysisCard,
        PredictionCard
    }
}
</script>