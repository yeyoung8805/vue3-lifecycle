<template>
  <h1 @click="increase">{{ count }}</h1>
  <h1 @click="changeMessage">{{ message }}</h1>
</template>

<script>
import { ref } from "vue";
export default {
  setup() {
    let count = ref(0);
    let message = ref("Hello world!");

    return {
      count,
      message,
    };
  },
};
</script>
