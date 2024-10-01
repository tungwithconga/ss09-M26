<template>
  <div>
    Email: <input type="text" v-model="email">
    Giá trị : {{email}}
  </div>
</template>

<script setup>
import { ref} from 'vue';
const email = ref("");

</script>

<style>

</style>