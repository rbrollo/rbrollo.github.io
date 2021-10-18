<template>
  <login-template>
    <span slot="menuesquerda">
      <img
        class="responsive-img"
        src="https://media.istockphoto.com/vectors/icon-vector-id849863560?k=20&m=849863560&s=612x612&w=0&h=H8e_3mFmDMWqLGceCBx_gM_n_L0DKECJO1BfNfI0ZEw="
        alt=""
      />
    </span>

    <span slot="principal">
      <h2>Cadastro</h2>
      <input type="text" placeholder="Nome" />
      <input type="text" placeholder="E-mail" />
      <input type="password" placeholder="Senha" />
      <input type="password" placeholder="Confirme sua Senha" />
      <button class="btn">Enviar</button>
      <router-link class="btn orange" to="/login">Já possuo conta </router-link>


    </span>
  </login-template>
</template>

<script>
import LoginTemplate from "@/templates/LoginTemplate.vue";
export default {
  components: { LoginTemplate },
  name: "Cadastro",
  data() {
    return {};
  },
};
</script>
<style scoped>
img {
  padding: 20px;
}

</style>
