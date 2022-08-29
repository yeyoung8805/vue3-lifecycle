<template>
  <div
    :class="{ large: large }"
    :style="{ backgroundColor: color }"
    class="btn"
  >
    Apple
  </div>
</template>

<script>
export default {
  props: {
    color: {
      type: String,
      default: "gray",
    },
    large: {
      type: Boolean,
      default: false,
    },
  },
};
</script>

<style scoped lang="scss">
.btn {
  display: inline-block;
  margin: 4px;
  padding: 6px 12px;
  border-radius: 4px;
  background-color: gray;
  color: white;
  cursor: pointer;
}
.btn.large {
  font-size: 20px;
  padding: 10px 20px;
}
</style>
