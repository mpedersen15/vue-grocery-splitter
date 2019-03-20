<template>
  <ul class="transaction-list">
    <li
      v-for="transaction in transactions"
      v-bind:key="transaction.id"
    >{{transaction.user + " - " + transaction.amount}}</li>
  </ul>
</template>

<script>
export default {
  name: "TransactionList",
  props: {
    transactions: Array
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
