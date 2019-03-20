<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <TransactionList
      v-bind:transactions="[
      {
        id: 1,
        user: 1,
        amount: 15.5
      },
      {
        id: 2,
        user: 2,
        amount: 10.0
      }
    ]"
    />
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import TransactionList from "./components/TransactionList.vue";

export default {
  name: "app",
  components: {
    HelloWorld,
    TransactionList
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
