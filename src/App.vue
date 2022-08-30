<template>
  <h1 @click="increase">{{ count }}</h1>
  <h1 @click="changeMessage">{{ message }}</h1>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
      message: "Hello world!",
    };
  },
  methods: {
    increase() {
      this.count += 1;
    },
    changeMessage() {
      this.message = "Good?!";
    },
  },
};
</script>
