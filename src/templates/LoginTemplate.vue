<template>
  <span>
    <header>
      <nav-bar logo="Social" url="#/" cor="green darken-1">
        <li><a href="#/">Home</a></li>
        <li><a href="#/Login ">Entrar</a></li>
      </nav-bar>
    </header>

    <main>
      <div class="container">
        <div class="row">
            <grid-vue tamanho="8">
            <card-menu-vue>
              <slot name="menues"/>
            </card-menu-vue>
            </grid-vue>
            <grid-vue tamanho="4">
              <slot name="principal"/>
            </grid-vue>
        </div> 
      </div>
    </main>

  <footer-vue cor="green darken-1" logo="Social" descricao="Teste de Descrição" ano="2018">

    <li><a class="grey-text text-lighten-3" href="#!">Home</a></li>
    <li><a class="grey-text text-lighten-3" href="#!">Link 2</a></li>
    <li><a class="grey-text text-lighten-3" href="#!">Link 3</a></li>
    <li><a class="grey-text text-lighten-3" href="#!">Link 4</a></li>
  </footer-vue>
  
  </span>
</template>

<script>
import NavBar from '@/components/layouts/NavBar'
import FooterVue from '@/components/layouts/FooterVue'
import GridVue from '@/components/layouts/GridVue'
import CardMenuVue from '@/components/layouts/CardMenuVue'

export default {
  name: "LoginTemplate",
  components: {
    NavBar,
    FooterVue,
    GridVue,
    CardMenuVue
  }
};
</script>

<style> 
</style>
