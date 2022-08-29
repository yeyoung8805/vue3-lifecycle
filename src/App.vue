<template>
  <div class="parent" @click="handler">
    <div class="child"></div>
  </div>
</template>

<script>
export default {
  methods: {
    handler(event) {
      console.log(event);
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
  overflow: auto; /* parent 영역 넘치는 child 영역이 있을 경우, scroll bar 생성함*/
  .child {
    width: 100px;
    height: 2000px;
    background-color: orange;
  }
}
</style>
