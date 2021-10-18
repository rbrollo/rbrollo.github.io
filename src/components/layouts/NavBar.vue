<template>
  <nav class="blue lighten-2">
    <div class="nav-wrapper container">
      <router-link class="brand-logo" to="/">
        <img
          src="https://media.istockphoto.com/vectors/icon-vector-id849863560?k=20&m=849863560&s=612x612&w=0&h=H8e_3mFmDMWqLGceCBx_gM_n_L0DKECJO1BfNfI0ZEw="
          alt=""
      /></router-link>
      <slot />
    </div>
  </nav>
</template>
<script>
export default {
  name: "NavBar",
};
</script>

<style scoped>
img {
  width: 80px;
}
</style>


