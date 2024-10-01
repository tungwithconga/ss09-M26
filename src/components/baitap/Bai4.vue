<template>
  <div>
    <p>Tiến độ hoàn thành: {{ progress }}%</p>
    <input type="range" v-model="progress" min="0" max="100" />

    <p>Sau khi thay đổi:</p>
    <p>Tiến độ hoàn thành: {{ progress }}%</p>
    <input type="range" v-model="progress" min="0" max="100" />
  </div>
</template>

<script setup>
import { ref } from 'vue';

const progress = ref(0); 
</script>

<style scoped>
input[type="range"] {
  width: 100%;
  margin: 10px 0;
}
</style>
