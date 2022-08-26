<template>
  <ul>
    <li v-for="(f, i) in fruits" :key="f">{{ f }}-{{ i + 1 }}</li>
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
