<!-- Strategy page with profile summary and introduction to me as a developer for Emprise. -->
<script setup lang="ts">
import StrategyDesign from '../components/StrategyPage/StrategyDesign.vue'
import StrategyDocumentation from '../components/StrategyPage/StrategyDocumentation.vue'
import StrategyRtm from '../components/StrategyPage/StrategyRtm.vue'

</script>
<template>
  
    <div>

      <h3 class="section-heading">Design Strategy</h3>
      <strategy-design />

      <p>&nbsp;</p><p>&nbsp;</p>
      <h3 class="section-heading">Requirement Traceability Matrix (RTM) Strategy</h3>
      <strategy-rtm />

      <p>&nbsp;</p><p>&nbsp;</p>

      <h3 class="section-heading">Documentation Strategy</h3>
      <strategy-documentation />

      
      <!-- Hold following data. -->

    </div>
  </template>

  
<style>
@media (min-width: 1024px) {
  .strategy {
    min-height: 50vh;
    /* display: flex;
    align-items: center;
    padding: inherit; */
  }
}
</style>