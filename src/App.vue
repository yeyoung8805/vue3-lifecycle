<template>
  <h1 @click="changeMessage">{{ msg }}</h1>
  <h1>{{ reversedMessage }}</h1>
</template>

<script>
export default {
  data() {
    return {
      msg: "Hello?",
    };
  },
  computed: {
    reversedMessage() {
      return this.msg.split("").reverse().join("");
    },
  },
  watch: {
    //newValue라는 변경된 값을 나타내는 변수명 자유롭게 사용 가능
    msg(newValue) {
      console.log("msg: ", this.newValue);
    },
    //마찬가지로 v라는 변경된 값을 나타내는 변수명 자유롭게 사용 가능
    reversedMessage(v) {
      console.log("reversedMessage: ", this.v);
    },
  },
  methods: {
    changeMessage() {
      this.msg = "Good!";
    },
  },
};
</script>
