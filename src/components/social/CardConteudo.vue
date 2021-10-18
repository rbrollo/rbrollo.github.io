<template>
  <div class="row">
    <!-- O card de fora -->
    <div class="card">
      <div class="card-content">
        <!-- Nome e foto em cima -->
        <div class="row valign-wrapper">
          <grid :tamanho="1">
            <img :src="img" :alt="nome" class="circle responsive-img" />
          </grid>
          <grid :tamanho="11">
            <span class="black-text">
              <strong>{{ nome }}</strong> - <small>{{ data }}</small>
            </span>
          </grid>
        </div>
        <!-- Nome e foto em cima -->
        <!-- Conteudo -->
        <slot />
        <!-- Conteudo -->
      </div>
      <div class="card-action">
        <p>
          <i class="material-icons">favorite_border</i>
          <i class="material-icons">insert_comment</i>
        </p>
      </div>
    </div>
  </div>

  <!-- O card de fora -->
</template>

<script>
import CardMenu from "../layouts/CardMenu.vue";
import Grid from "../layouts/Grid.vue";
export default {
  components: { CardMenu, Grid },
  name: "CardConteudo",
  props: ["img", "nome", "data"],
};
</script>

<style scoped>
p#nome {
  font-size: 0.9rem;
}
p {
  color: black;
}
</style>