<template>
  <!-- pages폴더에 파일을 추가하면, 
  .nuxt의 router.ts에 자동으로 추가됨 -->
  <div>
    <h1>메인 페이지</h1>
    <ul>
      <li v-for="product in products" :key="product.id">
        {{ product.name }} - {{ product.price }}원
      </li>
    </ul>
  </div>
</template>

<script setup lang="ts">
import axios from 'axios'
import { ref } from 'vue'

const products = ref([])

async function init() {
  try {
    const res = await axios.get('http://localhost:3000/products')
    products.value = res.data
  } catch (err) {
    console.error(err)
  }
}

init()
</script>

<style></style>
