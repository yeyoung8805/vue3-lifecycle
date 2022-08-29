<template>
  <MyBtn>Banana</MyBtn>
  <MyBtn :color="color" text="Banana" />
  <MyBtn large color="royalblue" text="Banana" />
  <MyBtn text="Banana" />
  <button>Banana</button>
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
