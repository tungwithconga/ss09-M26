<template>
  <div>
    <h1>One way data binding</h1>
    <h3>Username:{{ userName }}</h3>
    <input type="text" :value="userName">
    <button @click="handlechangeName">Change Name</button>
  </div>
</template>

<script setup>
import {ref} from "vue";
const userName = ref("Nguyen Van B");
const handlechangeName = () =>{
    userName.value = "Nguyen Van A";
}
</script>

<style>

</style>