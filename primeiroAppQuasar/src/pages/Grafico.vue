<template>
  <line-chart :data="data" />
</template>

<script>
import Vue from 'vue'
import Chartkick from 'vue-chartkick'
import Chart from 'chart.js'

Vue.use(Chartkick.use(Chart))

export default {
  name: 'grafico',
  data () {
    return {
      url: 'https://img.freepik.com/vetores-gratis/fundo-de-particulas-abstratas-tecnologia_52683-25766.jpg?size=626&ext=jpg',
      model: '',
      password: '',
      isPwd: true,
      data: [
        {
          name: 'Workout', data: { '2017-01-01 00:00:00 -0800': 3, '2017-01-02 00:00:00 -0800': 4 }
        },
        {
          name: 'Call parents', data: { '2017-01-01 00:00:00 -0800': 5, '2017-01-02 00:00:00 -0800': 3 }
        }]
    }
  }
}
</script>
