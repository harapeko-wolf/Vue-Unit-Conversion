<template>
  <div id="app"><UnitConversion /></div>
</template>

<script>
import UnitConversion from "./components/UnitConversion";

export default {
  name: "App",
  components: {
    UnitConversion
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
