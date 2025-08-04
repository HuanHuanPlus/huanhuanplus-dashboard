<template>
  <div class="min-h-screen bg-white text-center p-4">
    <h1 class="text-2xl font-bold text-purple-700 mb-2">Selamat Datang di HuanHuan Plus</h1>
    <p class="text-gray-600 mb-6">Dashboard Penjualan Otomatis & Produk Laris Shopee</p>

    <!-- Menu Sub-Bisnis -->
    <div class="grid grid-cols-1 sm:grid-cols-3 gap-4 mb-6">
      <NuxtLink to="/glowup" class="p-4 bg-pink-100 rounded-xl shadow hover:bg-pink-200">
        🧴 HuanHuan GlowUp
      </NuxtLink>
      <NuxtLink to="/gadget" class="p-4 bg-blue-100 rounded-xl shadow hover:bg-blue-200">
        📱 HuanHuan Gadget ID
      </NuxtLink>
      <NuxtLink to="/otto" class="p-4 bg-yellow-100 rounded-xl shadow hover:bg-yellow-200">
        🚗 HuanHuan Otto
      </NuxtLink>
    </div>

    <!-- Fitur Dashboard -->
    <div class="grid grid-cols-1 gap-4">
      <NuxtLink to="/produk-laris" class="p-4 bg-green-100 rounded-xl shadow hover:bg-green-200">
        🔍 Cari Produk Laris Shopee
      </NuxtLink>
      <NuxtLink to="/produk-saya" class="p-4 bg-gray-100 rounded-xl shadow hover:bg-gray-200">
        📦 Lihat Produk Tersimpan
      </NuxtLink>
      <NuxtLink to="/pengaturan" class="p-4 bg-purple-100 rounded-xl shadow hover:bg-purple-200">
        ⚙️ Pengaturan
      </NuxtLink>
    </div>
  </div>
</template>

<script setup>
</script>
