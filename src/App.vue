<template>
  <div @click="increase">{{ count }}</div>
</template>

<script>
export default {
  setup() {
    let count = 0,
    function increase() {
      count += 1;
    }
    return {
      count,
      increase
    }
  }
};
</script>
