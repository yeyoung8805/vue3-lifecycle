<template>
  <h1 @click="increase">{{ count }}</h1>
  <h1 @click="changeMessage">{{ message }}</h1>
</template>

<script>
export default {
  setup() {
    let count = 0;
    let message = "Hello world!";
  },
};
</script>
