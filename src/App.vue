<script setup>
import SB from './components/sidebar.vue'
</script>

<template>
  <SB id="sbc"/>
</template>

<style>
#app {
  display: grid;
  grid-template-rows: repeat(10, 1fr);
  grid-template-columns: repeat(10, 1fr);
}

#sbc {
  grid-area: 1 / 1 / 11 / 3;
  height: 100vh;
}
</style>
