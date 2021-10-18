<template>
  <div class="card-panel grey lighten-5 z-depth-1">
    <slot></slot>
  </div>
</template>
<script>
export default {
  name: "CardMenu",
};
</script>

<style  scoped>
div {
  display: flex;
  align-items: center;
  height: 150px;

}
</style>
