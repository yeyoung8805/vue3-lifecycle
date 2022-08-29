<template>
  <button @click="handler">Click 1</button>
  <button @click="handler">Click 2</button>
</template>

<script>
export default {
  methods: {
    handler(msg) {
      console.log(msg);
    },
  },
};
</script>
