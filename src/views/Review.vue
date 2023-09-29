<script setup>
import {ref} from 'vue'
</script>

<template>

  <div class="row g-5">
    <div class="col-md-8">
      <h3 class="pb-4 mb-4 fst-italic border-bottom">
        รีวิว
      </h3>

      <div class="blog-post" v-for="(item, index) in Review" :key="index">
          <article>
          <h2 class="display-5 link-body-emphasis mb-1">{{ item.title }}</h2>
          <p class="blog-post-meta">update {{ item.date}}</p>
          <hr>
          <blockquote class="blockquote">
            <p>ได้คะแนนรีวิว</p>
          </blockquote>
        </article>


        <article class="blog-post">
          <table class="table">
            <thead>
              <tr>
                <th>ชื่อ</th>
                <th>ราคา</th>
                <th>ความสะอาด</th>
                
                
              </tr>
            </thead>
            <tbody v-for="i in 5">
              <tr>
                <td>{{score[i].name}}</td>
                <td>{{score[i].price}}</td>
                <td>{{score[i].clean}}</td>
                
                
              </tr>
            </tbody>
          </table><br><br>
        </article>

      </div>

      
    </div>
  </div>
</template>

<script>
const Review = ref([
  {
    title: 'ร้านกาแฟดำ',
    date : 'December 18, 2023',
  },
  {
    title: 'ร้านกาแฟฟ้า',
    date : 'December 19, 2023',
  },
  {
    title: 'ร้านกาแฟเขียว',
    date : 'December 20, 2023',
  },
  {
    title: 'ร้านกาแฟแดง',
    date : 'December 21, 2023',
  },
  {
    title: 'ร้านกาแฟเหลือง',
    date : 'December 22, 2023',
  },
]);

const score = ref([
  {
    name:'',
    price: '',
    clean: ''
    
  },
  {
    name:'Kojo satoru',
    price: '9',
    clean: '9'
  },
  {
    name: 'Aren yager',
    price: '10',
    clean: '9'
  },
  {
    name: 'Naruto',
    price: '8',
    clean: '10'
  },
  {
    name: 'lnw tt',
    price: '10',
    clean: '10'
  },
  {
    name: 'Khp',
    price: '8',
    clean: '10'
  },
]);
</script>

<style scoped>

</style>