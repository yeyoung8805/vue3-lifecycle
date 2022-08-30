<template>
  <div class="btn">
    <slot></slot>
  </div>
  <h1 @click="$emit('click')">ABC</h1>
</template>

<script>
export default {
  emits: ["click"],
};
</script>

<style scoped>
.btn {
  display: inline-block;
  margin: 4px;
  padding: 6px 12px;
  border-radius: 4px;
  background-color: gray;
  color: white;
  cursor: pointer;
}
</style>
