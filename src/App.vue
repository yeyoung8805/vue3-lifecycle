<template>
  <h1 ref="hello">Hello world!</h1>
</template>

<script>
export default {
  mounted() {
    console.log(this.$refs.hello);
  },
};
</script>
