<template>
    <v-list subheader two-line>
      <v-list-item
        v-for="testCategory in testCategorys"
        :key="testCategory.title"
        :class="testCategory.index == 0 ? ' ': 'mt-n5'"
      >
        <v-list-item-content>
          <v-list-item-title v-text="testCategory.title">
          </v-list-item-title>
        </v-list-item-content>
        <v-list-item-action>
          <v-btn icon>
             <v-chip >5</v-chip>
          </v-btn>
        </v-list-item-action>
      </v-list-item>
    </v-list>
</template>
<script>

export default{
    name:"TotalTestList",
    data: () => ({
    
      testCategorys: [
        {
          title: 'Heat Tests',
          index:0
        },
        {
          title: 'Capacity Tests',
          index:1
        },
        {
          title: 'Voltage Tests',
          index:2
        },
      ],
    }),
    
}
</script>
