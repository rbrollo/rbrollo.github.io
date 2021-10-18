<template>
  <span>
    <div class="card-image">
      <img :src="img || ''" />
      <span class="card-title">{{ titulo || "" }}</span>
    </div>
    <div class="card-content">
      <p>
        {{ txt || "" }}
      </p>
    </div>
  </span>
</template>

<script>
export default {
  components: {},
  name: "CardDetalhe",
  props: ["txt", "titulo", "img"],
};
</script>

<style scoped>
</style>