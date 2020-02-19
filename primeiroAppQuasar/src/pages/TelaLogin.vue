<template>
    <q-page>
        <div class="row">
            <div class="col-4">
              <div class="row cadastro">
                <div class="col">
                  <q-card class="q-pa-lg q-ma-xl text-h4">
                    Faça seu login
                    <br><br>
                    <q-input
                      ref="input"
                      filled
                      v-model="model"
                      label="Login"
                      :rules="[val => !!val || 'O login é obrigatório']"
                    />
                     <q-input v-model="password" filled :type="isPwd ? 'password' : 'text'"
                     :rules="[val => !!val || 'A senha é obrigatória']"
                     ref= "input"
                     label="Senha"
                     >
                      <template v-slot:append>
                        <q-icon
                          :name="isPwd ? 'visibility_off' : 'visibility'"
                          class="cursor-pointer"
                          @click="isPwd = !isPwd"
                        />
                      </template>
                    </q-input>
                    <br>
                    <q-btn class="on-left" color="primary" label="Entrar" />
                  </q-card>
                </div>
              </div>
            </div>
            <div class="col-8 logo">
              <canvas id="myChart"></canvas>
            </div>
        </div>
    </q-page>
</template>

<style scoped>
.cadastro{
    border: 1px solid red;
    height: 100vh;
    justify-content: center;
    align-items: center;
}
.logo{
    border: 1px solid blue;
    height: 100vh;
}
</style>

<script>
export default {
  name: 'TelaLogin',
  data () {
    return {
      url: 'https://img.freepik.com/vetores-gratis/fundo-de-particulas-abstratas-tecnologia_52683-25766.jpg?size=626&ext=jpg',
      model: '',
      password: '',
      isPwd: true
    }
  }
}
</script>
