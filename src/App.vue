<template>
  <h1 @click="add">
    {{ msg }}
  </h1>
</template>

<script>
export default {
  data() {
    return {
      msg: "Hello World!",
    };
  },
  methods: {
    add() {
      this.msg += "!";
    },
  },
};
</script>
