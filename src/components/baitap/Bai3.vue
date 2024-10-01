<template>
  <div>
    <input type="date" v-model="date">
    Giá trị : {{date}}

  </div>
</template>

<script setup>
import { ref} from 'vue';
const date = ref(0);

</script>

<style>

</style>