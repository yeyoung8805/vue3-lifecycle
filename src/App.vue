<template>
  <h1>{{ reverseMessage() }}</h1>
  <h1>{{ reverseMessage() }}</h1>
  <h1>{{ reverseMessage() }}</h1>
  <h1>{{ reverseMessage() }}</h1>
</template>

<script>
export default {
  data() {
    return {
      msg: "Hello Computed!",
    };
  },
  methods: {
    reverseMessage() {
      this.msg.split("").reverse().join("");
    },
  },
};
</script>
