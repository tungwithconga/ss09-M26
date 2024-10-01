<template>
  <div>
    <h3>Trước khi người dùng lựa chọn:</h3>
    <div>
      <label>Sở thích</label>
      <div>
        <input type="checkbox" id="soccer" value="Đá bóng" v-model="selectedHobbies" />
        <label for="soccer">Đá bóng</label>
      </div>
      <div>
        <input type="checkbox" id="volleyball" value="Bóng chuyền" v-model="selectedHobbies" />
        <label for="volleyball">Bóng chuyền</label>
      </div>
      <div>
        <input type="checkbox" id="code" value="Code" v-model="selectedHobbies" />
        <label for="code">Code</label>
      </div>
      <div>
        <input type="checkbox" id="swimming" value="Bơi lội" v-model="selectedHobbies" />
        <label for="swimming">Bơi lội</label>
      </div>
    </div>

    <h3>Sau khi người dùng lựa chọn:</h3>
    <p>Sở thích: {{ selectedHobbies }}</p>
    <div>
      <input type="checkbox" id="soccer2" value="Đá bóng" v-model="selectedHobbies" />
      <label for="soccer2">Đá bóng</label>
      
      <input type="checkbox" id="volleyball2" value="Bóng chuyền" v-model="selectedHobbies" />
      <label for="volleyball2">Bóng chuyền</label>
      
      <input type="checkbox" id="code2" value="Code" v-model="selectedHobbies" />
      <label for="code2">Code</label>
      
      <input type="checkbox" id="swimming2" value="Bơi lội" v-model="selectedHobbies" />
      <label for="swimming2">Bơi lội</label>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue';

const selectedHobbies = ref([]);
</script>
