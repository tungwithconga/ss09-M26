<template>
  <div>
    <h3>Trước khi người dùng lựa chọn:</h3>
    <div>
      <label>Giới tính:</label>
      <input type="radio" id="male" value="Nam" v-model="selectedGender" />
      <label for="male">Nam</label>
      
      <input type="radio" id="female" value="Nữ" v-model="selectedGender" />
      <label for="female">Nữ</label>
      
      <input type="radio" id="other" value="Khác" v-model="selectedGender" />
      <label for="other">Khác</label>
    </div>

    <h3>Sau khi người dùng lựa chọn:</h3>
    <p>Giới tính: {{ selectedGender }}</p>
    <div>
      <input type="radio" id="male2" value="Nam" v-model="selectedGender" />
      <label for="male2">Nam</label>
      
      <input type="radio" id="female2" value="Nữ" v-model="selectedGender" />
      <label for="female2">Nữ</label>
      
      <input type="radio" id="other2" value="Khác" v-model="selectedGender" />
      <label for="other2">Khác</label>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const selectedGender = ref('');
</script>
