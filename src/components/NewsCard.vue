<script setup>
import { ref } from 'vue';
import { RouterLink } from 'vue-router'

</script>

<template>
  <div class="row mb-2">
    <div class="row g-0 border rounded overflow-hidden flex-md-row mb-4 shadow-sm h-md-250 position-relative">
      <div class="card" style="margin-left: 30px; margin: auto; padding: auto;" v-for="(item, index) in ShopList" :key="index">
        <RouterLink :to="{name: 'info', params: {id: index}}">
          <img :src="item.imageUrl">
        </RouterLink>
        <p style="font-size: 20px;">ร้าน {{ item.title }}</p>
        
      </div>
    </div>
    
  </div>
    
</template>

<script>
const ShopList = ref([
  {
    title: 'กาแฟดำ',
    imageUrl: 'image/coffee1.jpg',
    
  },
  {
    title: 'กาแฟฟ้า',
    imageUrl: 'image/coffee2.jpg',
    
  },
  {
    title: 'กาแฟเขียว',
    imageUrl: 'image/coffee3.jpg',
    
  },
  {
    title: 'กาแฟแดง',
    imageUrl: 'image/coffee4.jpg',
    
  },
  {
    title: 'กาแฟเหลือง',
    imageUrl: 'image/coffee5.jpg',
    
  },
]);
</script>


<style scoped>
body {
  font-family: Arial, sans-serif;
  
}

img{
  width: 250px;
  height: 200px;
}
.card {
  width: 250px;
  margin: 5px;
  padding: auto;
  text-align: center;
 
}
.card-container {
  position:fixed;
  padding: 20px;
  width: 200%;
}

.popup {
  display: none;
  position: fixed;
  width: 100%;
  height: 100%;
  align-items: center;
}

.popup-content {
  padding: 20px;
  text-align: center;
}


form {
  display: flex;
  flex-direction: column;
  gap: 10px;
}

label {
  font-weight: bold;
}

input {
  padding: 5px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  padding: 5px 15px;
  color: white;
  border: none;
}

.buttonc {
  padding: 5px 15px;
  background-color: #d50202;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}


button:hover {
  background-color: #0056b3;
}
</style>
