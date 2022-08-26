<template>
  <button @click="add">ADD</button>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
  <h1>{{ reversedMessage }}</h1>
</template>

<script>
export default {
  data() {
    return {
      //Getter , Setter
      msg: "Hello Computed!",
    };
  },
  computed: {
    //computed 메소드는 캐싱 되어 있기 때문에, 한번 계산하면 다시 반복해서 계산하지 않는다.
    //computed is read-only
    //= Getter
    // reversedMessage() {
    //   return this.msg.split("").reverse().join("");
    // },

    //Getter, Setter
    reversedMessage: {
      get() {
        return this.msg.split("").reverse().join("");
      },
      set(value) {
        this.msg = value;
      },
    },
  },
  methods: {
    add() {
      this.reversedMessage += "!?"; //computed 안에 들어있는 메소드 이므로 변경사항 반영이 안된다.
      // this.msg += "!?"; //data 안에 들어있는 데이터이므로 변경가능 하다.
    },
  },
};
</script>
