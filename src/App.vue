<template>
  <h1 id="hello">Hello world!</h1>
</template>

<script>
export default {
  mounted() {
    const h1El = document.querySelector("#hello");
    console.log(h1El.textContent);
  },
};
</script>
