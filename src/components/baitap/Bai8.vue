<template>
  <div>
    <h3>Thêm mới tài khoản</h3>
    <form @submit.prevent="register">
      <div>
        <label for="name">Họ và tên</label>
        <input type="text" id="name" v-model="user.name" placeholder="Nhập họ và tên" />
      </div>
      
      <div>
        <label for="email">Email</label>
        <input type="email" id="email" v-model="user.email" placeholder="Nhập email" />
      </div>
      
      <div>
        <label for="password">Mật khẩu</label>
        <input type="password" id="password" v-model="user.password" placeholder="Nhập mật khẩu" />
      </div>
      
      <div>
        <label for="confirmPassword">Nhập lại mật khẩu</label>
        <input type="password" id="confirmPassword" v-model="user.confirmPassword" placeholder="Nhập lại mật khẩu" />
      </div>
      
      <button type="submit">Đăng ký</button>
    </form>
  </div>
</template>

<script setup>
import { reactive } from 'vue';

const user = reactive({
  name: '',
  email: '',
  password: '',
  confirmPassword: ''
});

const register = () => {
  if (user.password === user.confirmPassword) {
    console.log('Dữ liệu người dùng:', user);
  } else {
    console.error('Mật khẩu không khớp');
  }
};
</script>
