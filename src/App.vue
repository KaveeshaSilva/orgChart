<template>
  <div id="app">
    <Header/>
    <OrgChart/>
    <!-- <test/> -->

   
  </div>
</template>

<script>

 
  import OrgChart from './composant/OrgChart.vue'

  export default {

    components: { 
      OrgChart,
    },

    name: 'app',
    data () {
      return {
      }
    }
  }
</script>

<style lang="scss" src="./style/app.css">
</style>





