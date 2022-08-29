<template>
  <input type="text" @keydown="handler" />
</template>

<script>
export default {
  methods: {
    handler(event) {
      if (event.key === "Enter") {
        console.log("Enter!!");
      }
    },
  },
};
</script>
