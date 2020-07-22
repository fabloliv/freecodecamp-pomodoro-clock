<template>
  <v-card>
    <v-tabs v-model="timerType">
      <v-tab
        v-for="tab in tabTitles"
        :key="tab"
      >
        {{ tab }}
      </v-tab>
    </v-tabs>
  </v-card>
</template>

<script>
export default {
  data() {
    return {
        timerType: 0,
        tabTitles: ['Pomodoro', 'Short Break', 'Long Break']
    }
  }
}
</script>