<template>
  <div>
    <h3>Thêm mới sản phẩm</h3>
    <form @submit.prevent="addProduct">
      <div>
        <label for="productCode">Mã sản phẩm</label>
        <input type="text" id="productCode" v-model="product.code" placeholder="Nhập mã sản phẩm" />
      </div>
      
      <div>
        <label for="productName">Tên sản phẩm</label>
        <input type="text" id="productName" v-model="product.name" placeholder="Nhập tên sản phẩm" />
      </div>
      
      <div>
        <label for="price">Giá</label>
        <input type="number" id="price" v-model="product.price" placeholder="Nhập giá sản phẩm" />
      </div>
      
      <div>
        <label for="quantity">Số lượng</label>
        <input type="number" id="quantity" v-model="product.quantity" placeholder="Nhập số lượng sản phẩm" />
      </div>
      
      <button type="submit">Thêm mới</button>
    </form>
  </div>
</template>

<script setup>
import { reactive } from 'vue';

const product = reactive({
  code: '',
  name: '',
  price: 0,
  quantity: 0
});

const addProduct = () => {
  console.log('Dữ liệu sản phẩm:', product);
};
</script>
