<template>
  <ul>
    <li v-for="(f, i) in fruits" :key="f">{{ f }}-{{ i }}</li>
  </ul>
</template>

<script>
export default {
  data() {
    return {
      fruits: ["Apple", "Banana", "Cherry"],
    };
  },
};
</script>
