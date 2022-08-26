<template>
  <ul>
    <li v-for="(fruit, index) in fruits" :key="fruit">
      {{ fruit }}-{{ index }}
    </li>
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
