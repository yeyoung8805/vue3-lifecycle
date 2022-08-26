<template>
  <h1 :style="fontStyle" @click="changeStyle">Hello?!</h1>
</template>

<script>
export default {
  data() {
    return {
      fontStyle: {
        color: "orange",
        fontSize: "30px",
      },
    };
  },
  methods: {
    changeStyle() {
      this.fontStyle.color = "red";
      this.fontStyle.fontSize = "50px";
    },
  },
};
</script>
