<template>
  <div id="app">
    <h2>Making radio components</h2>
    <custom-radio name="radio-1" />
    <custom-radio name="radio-1" />
  </div>
</template>

<script>
import CustomRadio from "./components/CustomRadio";

export default {
  name: "App",
  components: { CustomRadio },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
