<template>
  <section v-if="fruits.length > 0">
    <h1>Fruits</h1>
    <ul>
      <li v-for="fruit in fruits" :key="fruit">
        {{ fruit }}
      </li>
    </ul>
  </section>
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
