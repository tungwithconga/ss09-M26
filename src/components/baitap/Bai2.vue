<template>
  <div>
    <p>Trước khi người dùng chọn màu:</p>
    <div :style="{ backgroundColor: selectedColor, width: '100px', height: '50px', border: '1px solid black' }"></div>
    <p>Mã màu: {{ selectedColor }}</p>
    
    <p>Sau khi người dùng chọn màu:</p>
    <input type="color" v-model="selectedColor" />
    <div :style="{ backgroundColor: selectedColor, width: '100px', height: '50px', border: '1px solid black' }"></div>
    <p>Mã màu: {{ selectedColor }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const selectedColor = ref('#000000');
</script>

<style scoped>
div {
  margin-bottom: 10px;
}
</style>
