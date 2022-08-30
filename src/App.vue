<template>
  <Parent />
</template>

<script>
import Parent from "~/components/Parent";
export default {
  components: {
    Parent,
  },
  data() {
    return {
      message: "Hello World!",
    };
  },
  provide() {
    return {
      msg: this.message,
    };
  },
};
</script>
