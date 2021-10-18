<template>
  <div class="row">
    <grid class="input-field" tamanho="12">
      <textarea v-model="conteudo" class="materialize-textarea"></textarea>
      <label>Lansa</label>
    </grid>

    <grid
      v-if="conteudo"
      class="btn waves-effect waves-light"
      tamanho="2 offset-s10"
    >
      Publicar
    </grid>
  </div>
</template>

<script>
import Grid from "../layouts/Grid.vue";

export default {
  components: { Grid },
  name: "PublicarConteudo",
  props: [],
  data() {
    return {
      conteudo: "",
    };
  },
};
</script>

<style scoped>
</style>