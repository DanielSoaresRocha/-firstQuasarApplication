<template>
  <q-page class="q-pa-xl">
    <div class="logo text-h4">O primeiro sistema Web Quasar</div>
    <div class="row justify-center">
      <q-card class="col-4 q-ma-xl q-pa-sm cards">
        <div class="text-h6 text">
          O que irei aprender?
        </div>
        <br><br>
        <div class="text-body1 text">
          Como criar um app utilizando Quasar, Vue.js, Vuex, axios. Utilizando conhecimentos
          adquiridos por video aulas práticas e teóricas
        </div>
      </q-card>
      <q-card class="col-4 q-ma-xl q-pa-sm cards">
        <div class="text-h6 text">
          E como começar?
        </div>
        <br><br>
        <div class="text-body1 text">
          Pelo começo, mas pretendo começar codificando e aprendendo a partir da documentação. Bem
          como utilizando conhecimentos adquiridos em experiências anteriores
        </div>
      </q-card>
    </div>
  </q-page>
</template>

<style lang="scss">
.logo{
  /*border:1px solid black;*/
  text-align: center;
}
.cards{
  color: $teal-8;
  background-color: $teal-8;
}
.text{
  color:white;
}
</style>

<script>
export default {
  name: 'PageIndex'
}
</script>
