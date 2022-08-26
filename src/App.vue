<template>
  <h1>{{ msg.split("").reverse().join("") }}</h1>
</template>

<script>
export default {
  data() {
    return {
      msg: "Hello Computed!",
    };
  },
};
</script>
