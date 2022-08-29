<template>
  <h1>{{ msg }}</h1>
  <input type="text" v-model.lazy="msg" />
</template>

<script>
export default {
  data() {
    return {
      msg: "Hello world!",
    };
  },
};
</script>
