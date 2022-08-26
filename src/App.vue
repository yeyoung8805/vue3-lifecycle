<template>
  <button @click="handler">Click me!</button>
  <h1 v-if="isShow">Hello?!</h1>
</template>

<script>
export default {
  data() {
    return {
      isShow: true,
    };
  },
  methods: {
    handler() {
      this.isShow = !this.isShow;
    },
  },
};
</script>
