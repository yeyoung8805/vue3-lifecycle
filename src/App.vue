<template>
  <div class="parent" @click="handlerA">
    <div class="child"></div>
  </div>
</template>

<script>
export default {
  methods: {
    handlerA(event) {
      console.log(event.target);
      console.log(event.currentTarget);
      console.log("A");
    },
    handlerB() {
      console.log("B");
    },
  },
};
</script>

<style scoped lang="scss">
.parent {
  width: 200px;
  height: 100px;
  background-color: royalblue;
  margin: 10px;
  padding: 10px;
  .child {
    width: 100px;
    height: 100px;
    background-color: orange;
  }
}
</style>
