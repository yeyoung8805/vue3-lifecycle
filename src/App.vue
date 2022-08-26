<template>
  <ul>
    <li v-for="fruit in newFruits" :key="fruit.id">{{ fruit.name }}</li>
  </ul>
</template>

<script>
import shortid from "shortid";
export default {
  data() {
    return {
      fruits: ["Apple", "Banana", "Cherry"],
      // newFruits: [
      //   { id: 0, name: "Apple" },
      //   { id: 1, name: "Banana" },
      //   { id: 2, name: "Cherry" },
      // ],
    };
  },
  computed: {
    newFruits() {
      return this.fruits.map((fruit) => ({
        id: shortid.generate(),
        name: fruit,
      }));
    },
  },
};
</script>
