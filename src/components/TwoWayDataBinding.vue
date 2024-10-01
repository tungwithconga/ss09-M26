<template>
  <form @submit="handleSubmit">
    <h2>UserName:{{userName}}</h2>
    <h2>Date Of Birth:{{ date }}</h2>
    <h2>Gender: {{gender}}</h2>
    <h3>Thêm mới người dùng</h3>
    <div>Họ và tên: <input v-model="userName" type="text" placeholder="Nhap ten"></div>
    <div>Ngày sinh: <input v-model="date" type="date"></div>
    <div>Giới tính:</div>
    <div>
        Nam <input v-model="gender" type="radio"> 
        Nữ <input v-model="gender" type="radio"> 
        Khác <input v-model="gender" type="radio">
    </div>
    <div>Sở thích</div>
    <div>
        Chơi game <input v-model="hobies" type="checkbox">
        Code <input type="checkbox">
        Thể thao <input type="checkbox">
        Đi du lịch <input type="checkbox">
    </div>
    <button>Thêm</button>
  </form>
</template>

<script setup>
import { ref} from "vue";
const userName = ref("");
const date = ref("");
const gender = ref("");
const hobies = ref("");
const handleSubmit = (e) =>{
    e.preventDefault();
}
</script>

<style>

</style>