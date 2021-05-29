<template>
  <div id="app">
    <img src="https://cdn2.iconfinder.com/data/icons/crane-1/500/vab810_12_construction_crane_excavator_isometric_cartoon_business_car-512.png">
    <UnderConstruction />
  </div>
</template>

<script>
import UnderConstruction from "./components/UnderConstruction";

export default {
  name: 'App',
  components: {
    UnderConstruction
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
