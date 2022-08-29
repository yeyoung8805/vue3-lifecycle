<template>
  <button @click="handler('hi')">Click 1</button>
  <button @click="handler('what')">Click 2</button>
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
