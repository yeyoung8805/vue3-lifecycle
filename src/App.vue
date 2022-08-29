<template>
  <input type="text" @keydown.a.ctrl="handler" />
</template>

<script>
export default {
  methods: {
    handler() {
      console.log("Enter!!");
    },
  },
};
</script>
