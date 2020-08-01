<template>
  <div>
    <v-card outlined max-width="1000">
      <v-sparkline
        :value="value"
        :labels="labels"
        :gradient="gradient"
        :smooth="radius || false"
        :padding="padding"
        :line-width="width"
        :stroke-linecap="lineCap"
        :gradient-direction="gradientDirection"
        :fill="fill"
        :type="type"
        :auto-line-width="autoLineWidth"
        auto-draw
      ></v-sparkline>
    </v-card>
    <v-card outlined max-width="1000">
      <v-sparkline
        :value="value"
        :labels="labels"
        :gradient="gradient"
        :padding="padding"
        :line-width="width"
        :stroke-linecap="lineCap"
        :gradient-direction="gradientDirection"
        :fill="fill"
        :type="type"
        :auto-line-width="autoLineWidth"
        auto-draw
      ></v-sparkline>
    </v-card>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data: () => ({
    width: 1,
    radius: 10,
    padding: 8,
    lineCap: 'round',
    gradient: ['red', 'blue'],
    value: [4, 2, 5, 9, 5, 10, 3, 5, 0, 3],
    labels: [...Array(10).keys()].map((x) => x.toString()),
    gradientDirection: 'top',
    fill: false,
    type: 'trend',
    autoLineWidth: false
  })
})
</script>
