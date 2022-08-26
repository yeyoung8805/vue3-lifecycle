<template>
  <section v-if="hasFruit">
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
  computed: {
    //계산된 데이터
    hasFruit() {
      return this.fruits.length > 0;
    },
  },
};
</script>
