<template>
  <MyBtn />
  <MyBtn :color="color" />
  <MyBtn large color="royalblue" />
  <MyBtn />
</template>

<script>
import MyBtn from "~/components/MyBtn";
export default {
  components: {
    MyBtn,
  },
  data() {
    return {
      color: "#000",
    };
  },
};
</script>
