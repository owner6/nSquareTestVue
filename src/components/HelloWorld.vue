<template>
  <div class="hello">
    <h1>Квадрат числа</h1>
    <input v-model="number" type="number" placeholder="Введите число" />
    <button @click="calculateSquare">Вычислить квадрат</button>
    <p v-if="result !== null">Квадрат числа: {{ result }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      result: null,
    };
  },
  methods: {
    calculateSquare() {
      this.result = this.number ** 2;
    },
  },
};
</script>

<style scoped></style>
