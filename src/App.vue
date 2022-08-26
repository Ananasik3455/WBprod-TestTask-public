<!-- App.vue -->
<template>
  <v-app>
    
    <v-main>
      <v-container
        py-8 px-6
        mx-0
        fluid
      >
        <h5 
          class="text-h5 white--text"
        > Доставки </h5>
        <h6 
          class="text-subtitle-1 grey--text"
        > Как только выкуп оплачен, он моментально появится в доставках. Дальше мы отслеживаем его статус. "Доставлен" - можно забирать с пункта выдачи. </h6>
      </v-container>

      <Card></Card>
    </v-main>
    
  </v-app>
</template>

<style>

  .v-main {
    background: #1D1625;
  }

</style>

<script>
import Card from './components/Card.vue'

export default {
  name: 'App',
  data () {

  },
  components: {
    Card
  },
}
</script>