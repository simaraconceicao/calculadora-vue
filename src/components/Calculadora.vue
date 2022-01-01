<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
</script>

<template>
  <h1>{{ msg }}</h1>
  <div class='calculadora'>
    <div class='display'>0.8765</div>
    <div class='botao'>C</div>
    <div class='botao'>+/-</div>
    <div class='botao'>%</div>
    <div class='botao operadores'>/</div>
    <div class='botao'>7</div>
    <div class='botao'>8</div>
    <div class='botao'>9</div>
    <div class='botao operadores'>x</div>
    <div class='botao'>4</div>
    <div class='botao'>5</div>
    <div class='botao'>6</div>
    <div class='botao operadores'>-</div>
    <div class='botao'>1</div>
    <div class='botao'>2</div>
    <div class='botao'>3</div>
    <div class='botao operadores'>+</div>
    <div class='botao zero'>0</div>
    <div class='botao'>.</div>
    <div class='botao operadores'>=</div>
  </div>

</template>

<style scoped>
.calculadora {
  margin: 0 auto;
  width: 350px;
  font-size: 40px;
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-auto-rows: minmax(50px, auto);
}

.display {
  grid-column: 1 / 5;
  background-color: #333;
  color: white;
}

.zero {
  grid-column: 1 / 3;
}

.botao {
  background-color: plum;
  border: 1px solid rgb(247, 247, 247);
}

.operadores {
  background-color: rgb(159, 102, 159);
  color: white;
}
</style>
