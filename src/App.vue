<template>
  <h1>Hello world!</h1>
</template>

<script>
export default {
  mounted() {
    const h1El = document.querySelector("h1");
    console.log(h1El.textContent);
  },
};
</script>
