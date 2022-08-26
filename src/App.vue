<template>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
</template>

<script>
export default {
  data() {
    return {
      msg: "Hello Computed!",
    };
  },
  computed: {
    //computed 메소드는 캐싱 되어 있기 때문에, 한번 계산하면 다시 반복해서 계산하지 않는다.
    reversedMessage() {
      return this.msg.split("").reverse().join("");
    },
  },
};
</script>
