<template>
  <div class="chart-container">
    <chart height="100%" width="100%"/>
  </div>
</template>

<script lang="ts">
  import { Component, Vue } from 'vue-property-decorator';
  import {
    LineMarker as Chart
  } from '@/components';

  @Component({
    components: {
      Chart
    }
  })
  export default class LineChart extends Vue {
  }
</script>

<style scoped>
  .chart-container{
    position: relative;
    width: 100%;
    height: calc(100vh - 84px);
  }
</style>
