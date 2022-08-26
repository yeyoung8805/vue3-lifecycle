<template>
  <h1>{{ msg.split("").reverse().join("") }}</h1>
  <h1>{{ msg.split("").reverse().join("") }}</h1>
  <h1>{{ msg.split("").reverse().join("") }}</h1>
  <h1>{{ msg.split("").reverse().join("") }}</h1>
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
