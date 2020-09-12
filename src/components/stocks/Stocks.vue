<template>
  <div>
    <app-stock
      v-for="stock in stocks"
      :key="stock.id"
      :stock="stock"
    ></app-stock>
  </div>
</template>

<script>
import Stock from "./Stock";

export default {
  data() {
    return {
      stocks: [
        { id: 1, name: "BMW", price: 110 },
        { id: 2, name: "Google", price: 220 },
        { id: 3, name: "Twiter", price: 10 },
        { id: 4, name: "Apple", price: 130 },
        { id: 5, name: "Panasoni", price: 210 }
      ]
    };
  },
  components: {
    appStock: Stock
  }
};
</script>

<style></style>
