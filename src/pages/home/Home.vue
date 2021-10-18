<template>
  <site-template>
    <span slot="menuesquerda">
      <div class="row valign-wrapper">
        <grid :tamanho="4">
          <img
            src="https://avatars.githubusercontent.com/u/83840786?v=4"
            alt=""
            class="circle responsive-img"
          />
        </grid>
        <grid :tamanho="8">
          <span class="black-text">
            <h5>Rogério Brollo</h5>
            Add the "circle" class to it to make it appear circular.
          </span>
        </grid>
      </div></span
    >

    <span slot="principal">
      <publicar-conteudo />
      <card-conteudo
        img="https://avatars.githubusercontent.com/u/83840786?v=4"
        nome="Rogério Brollo"
        data="18/10/2021 09:05"
      >
        <card-detalhe
          txt="Teste de um texto lindo"
          titulo=""
          img="https://materializecss.com/images/sample-1.jpg"
        />
      </card-conteudo>
    </span>
  </site-template>
</template>

<script>
import Grid from "../../components/layouts/Grid.vue";
import CardConteudo from "../../components/social/CardConteudo.vue";
import CardDetalhe from "../../components/social/CardDetalhe.vue";
import PublicarConteudo from "../../components/social/PublicarConteudo.vue";
import SiteTemplate from "../../templates/SiteTemplate.vue";
export default {
  components: {
    CardConteudo,
    CardDetalhe,
    Grid,
    SiteTemplate,
    PublicarConteudo,
  },
  name: "Home",
  data() {
    return {};
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
