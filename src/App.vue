<template>
  <button @click="handler">Click me!</button>
</template>

<script>
export default {
  methods: {
    handler(e) {
      console.log(e);
      console.log(e.target.textContent);
    },
  },
};
</script>
