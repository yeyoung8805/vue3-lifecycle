<template>
  <h1>{{ msg }}</h1>
  <input type="text" v-model.number="msg" />
</template>

<script>
export default {
  data() {
    return {
      msg: 123,
    };
  },
  watch: {
    msg() {
      console.log(typeof this.msg);
    },
  },
};
</script>
