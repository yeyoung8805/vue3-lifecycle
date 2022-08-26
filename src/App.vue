<template>
  <h1 v-bind="msg">
    {{ msg }}
  </h1>
</template>

<script>
export default {
  data() {
    return {
      msg: "active",
    };
  },
  methods: {
    add() {
      this.msg += "!";
    },
  },
};
</script>

<style>
.active {
  color: royalblue;
  font-size: 100px;
}
</style>
