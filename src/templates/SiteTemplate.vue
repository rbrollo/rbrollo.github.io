<template>
  <span>
    <header>
      <nav-bar>
        <ul id="nav-mobile" class="right hide-on-med-and-down">
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/login">Entrar</router-link></li>
          <li><router-link to="/cadastro">Cadastre-se</router-link></li>

        </ul>
      </nav-bar>
    </header>
    <main>
      <div class="container">
        <div class="row">
          <grid :tamanho="4">
            <card-menu>
              <slot name="menuesquerda" />
            </card-menu>
          </grid>
          <grid :tamanho="8">
            <slot name="principal" />
          </grid>
        </div>
      </div>
    </main>
    <footer><rodape /></footer>
  </span>
</template>

<script>
import CardMenu from "@/components/layouts/CardMenu.vue";
import rodape from "@/components/layouts/Footer.vue";
import Grid from "@/components/layouts/Grid.vue";
import NavBar from "@/components/layouts/NavBar.vue";
import CardConteudo from "@/components/social/CardConteudo.vue";
export default {
  components: { NavBar, rodape, Grid, CardMenu, CardConteudo },
  name: "SiteTemplate",
};
</script>

<style>
</style>
