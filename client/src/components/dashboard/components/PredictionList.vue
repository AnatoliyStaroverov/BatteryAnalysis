<template>
    <v-list subheader two-line>
      <v-list-item
        v-for="testCategory in testCategorys"
        :key="testCategory.title"
        :class="testCategory.index == 0 ? ' ': 'mt-n5'"
      >
        <v-list-item-content>
          <v-list-item-title>
            <b>{{testCategory.title}}</b>
          </v-list-item-title>
         <p class="ml-2">{{testCategory.result}}
         </p>
        </v-list-item-content>
        <v-list-item-action>
          <v-btn icon>
             <v-chip >{{testCategory.accuracy}}</v-chip>
          </v-btn>
        </v-list-item-action>
      </v-list-item>
    </v-list>
</template>
<script>

export default{
    name:"PredictionList",
    data: () => ({
    
      testCategorys: [
        {
          title: 'Heat Prediction',
          index:0,
          result:"Higher temperture yeilds better Performance",
          accuracy:"90%"
        },
        {
          title: 'Capacity Prediction',
          index:1,
           result:"Capacity is Direcly related to Temperature",
            accuracy:"69%"
        },
        {
          title: 'Voltage Prediction',
          index:2,
           result:"Voltage is directly related to the distrubution of xyz...",
            accuracy:"88%"
        },
      ],
    }),
    
}
</script>
