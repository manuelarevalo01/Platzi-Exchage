<template>
  <main>
    <px-header :links="links" />

    <router-view class="container px-5 sm:px-20 py-20 flex justify-center" />
  </main>
</template>

<script>
import PxHeader from '@/components/PxHeader'

export default {
  name: 'app',
  components: { PxHeader },

  data() {
    return {
      links: [
        {
          title: 'BTC',
          to: { name: 'coin-detail', params: { id: 'bitcoin' } }
        },
        {
          title: 'ETH',
          to: { name: 'coin-detail', params: { id: 'ethereum' } }
        },
        {
          title: 'XRP',
          to: { name: 'coin-detail', params: { id: 'ripple' } }
        },
        {
          title: 'ADA',
          to: { name: 'coin-detail', params: { id: 'cardano' } }
        },
        {
          title: 'BNB',
          to: { name: 'coin-detail', params: { id: 'binance-coin' } }
        },
        {
          title: 'USDT',
          to: { name: 'coin-detail', params: { id: 'tether' } }
        },
        {
          title: 'DOGE',
          to: { name: 'coin-detail', params: { id: 'dogecoin' } }
        },
        {
          title: 'BCH',
          to: { name: 'coin-detail', params: { id: 'bitcoin-cash' } }
        },
        {
          title: 'ICP',
          to: { name: 'coin-detail', params: { id: 'litecoin' } }
        },
        {
          title: 'LTC',
          to: { name: 'coin-detail', params: { id: 'stellar' } }
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
