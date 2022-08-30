<template>
  <div class="btn">
    <slot></slot>
  </div>
  <h1 :class="$attrs.class" :style="$attrs.style"></h1>
</template>

<script>
export default {
  inheritAttrs: false,
  created() {
    console.log(this.$attrs);
  },
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
