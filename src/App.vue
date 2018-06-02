<template>
  <div id="app">
    <img src="./assets/logo.png">
    <TableSorter/>
  </div>
</template>

<script>
import TableSorter from "./components/TableSorter";

export default {
  name: "App",
  components: {
    TableSorter
  }
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
