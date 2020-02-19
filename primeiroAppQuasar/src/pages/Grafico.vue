<template>
    <pie-chart :data="[['Blueberry', 44], ['Strawberry', 23]]"></pie-chart>
</template>

<script>
import Vue from 'vue'
import Chartkick from 'vue-chartkick'
import Chart from 'chart.js'

Vue.use(Chartkick.use(Chart))

export default {
  name: 'grafico'
}

</script>
