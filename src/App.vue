<template>
  <MyBtn>
    <template v-slot:icon>
      <span>(B)</span>
    </template>
    <template v-slot:text>
      <span>Banana</span>
    </template>
  </MyBtn>
</template>

<script>
import MyBtn from "~/components/MyBtn";
export default {
  components: {
    MyBtn,
  },
};
</script>
