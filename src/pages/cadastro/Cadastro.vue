<template>

  <login-template>

      <span slot="menues">
         <img src="https://static.quizur.com/i/b/5b035c77702c13.471891555b035c775c3ff9.54480388.png" class="responsive-img">
      </span>
    
    <span slot="principal">

        <h2>Cadastro</h2>

        <input type="text" placeholder="Nome" value="">
        <input input="text" placeholder="E-mail" value="">
        <input type="password" placeholder="Senha" value="">
        <input type="password" placeholder="Confirme sua Senha" value="">
        <button class="btn">Enviar</button>
        <router-link class="btn orange" to="/login">Já tenho conta</router-link>

    </span>
  

  </login-template>
 


</template>

<script>
import LoginTemplate from '@/templates/LoginTemplate'

export default {
  name: 'Cadastro',
  data () {
    return {
    }
  },
  components: {
    LoginTemplate
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    
</style>
 