<template>
  <h1 :style="{ color: color, fontSize: fontSize }" @click="changeStyle">
    Hello?!
  </h1>
</template>

<script>
export default {
  data() {
    return {
      color: "orange",
      fontSize: "30px",
    };
  },
};
</script>
