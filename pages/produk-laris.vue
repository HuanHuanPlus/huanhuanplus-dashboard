<template>
  <div class="min-h-screen p-4 bg-white">
    <h1 class="text-2xl font-bold text-green-700 mb-4">🔍 Produk Laris Shopee</h1>

    <form @submit.prevent="cariProduk">
      <input v-model="toko" placeholder="Masukkan nama toko Shopee" class="p-2 border rounded w-full mb-4" />
      <button type="submit" class="bg-green-500 text-white px-4 py-2 rounded hover:bg-green-600">Cari Produk</button>
    </form>

    <div v-if="loading" class="mt-4 text-gray-500">⏳ Sedang mencari produk...</div>
    <div v-if="produk.length" class="mt-6 grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
      <div v-for="item in produk" :key="item.id" class="p-4 border rounded shadow">
        <img :src="item.gambar" class="w-full h-32 object-cover rounded mb-2" />
        <h2 class="font-semibold">{{ item.nama }}</h2>
        <p>Terjual: {{ item.terjual }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const toko = ref('')
const loading = ref(false)
const produk = ref([])

const cariProduk = async () => {
  loading.value = true
  produk.value = []

  // 👉 Nanti kita sambungkan ke API Scraper Shopee (otomatis)
  setTimeout(() => {
    produk.value = [
      { id: 1, nama: 'Some By Mi AHA BHA PHA 30 Days Miracle', terjual: '14.200', gambar: 'https://down-id.img.susercontent.com/file/sg-11134201-22100-z4g1az7hr1ivc3' },
      { id: 2, nama: 'Some By Mi Snail Truecica', terjual: '10.543', gambar: 'https://down-id.img.susercontent.com/file/sg-11134201-7qvdl-llwh78j1xvcr26' }
    ]
    loading.value = false
  }, 1500)
}
</script>
