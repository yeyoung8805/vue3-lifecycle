<template>
  <a href="https://naver.com" target="_blank" @click="handler"> Naver </a>
</template>

<script>
export default {
  methods: {
    handler(event) {
      event.preventDefault();
      console.log("ABC!");
    },
  },
};
</script>
