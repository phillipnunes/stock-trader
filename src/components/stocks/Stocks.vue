<template>
  <div>
    <app-stock v-for="stock in stocks" :stock="stock" :key="stock.id"></app-stock>
  </div>
</template>

<script>
import Stock from './Stock'

export default {
  data () {
    return {
      stocks: [
        {id: 1, name: 'AAA', price: 123},
        {id: 2, name: 'BBB', price: 1231},
        {id: 3, name: 'CCC', price: 2345},
        {id: 4, name: 'DDD', price: 654}
      ]
    }
  },
  components: {
    appStock: Stock
  }
}
</script>
