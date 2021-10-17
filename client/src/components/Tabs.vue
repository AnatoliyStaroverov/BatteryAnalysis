<template>
  <v-card class="mt-14">
    <v-tabs
      v-model="tab"
      background-color="primary"
      dark
      grow
    >
      <v-tab
        v-for="item in items"
        :key="item.tab"
      >
        {{ item.tab }}
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
        v-for="item in items"
        :key="item.tab"
      >
        <v-card flat>
          <v-card-text>{{ item.content }}</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>
  </v-card>
</template>

<script>
  export default {
    name: 'Tabs',
    data () {
      return {
        tab: null,
        items: [
          { tab: 'Input Tests', content: 'Tab 1 Content' },
          { tab: 'Calculator', content: 'Tab 2 Content' },
          { tab: 'Test Results', content: 'Tab 3 Content' },

        ],
      }
    },
  }
</script>


