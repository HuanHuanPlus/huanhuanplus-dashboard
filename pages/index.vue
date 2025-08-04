<template>
  <div class="min-h-screen bg-white text-gray-800 p-6">
    <h1 class="text-3xl font-bold mb-2">Selamat Datang di HuanHuan Plus</h1>
    <p class="text-lg text-gray-600 mb-8">
      Dashboard Penjualan Otomatis & Produk Laris Shopee
    </p>

    <!-- Menu Sub-Bisnis -->
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4 mb-8">
      <NuxtLink to="/glowup" class="p-4 border rounded shadow hover:bg-blue-50 text-center font-medium">
        🧴 HuanHuan GlowUp
      </NuxtLink>
      <NuxtLink to="/gadget" class="p-4 border rounded shadow hover:bg-blue-50 text-center font-medium">
        📱 HuanHuan Gadget ID
      </NuxtLink>
      <NuxtLink to="/otto" class="p-4 border rounded shadow hover:bg-blue-50 text-center font-medium">
        🚗 HuanHuan Otto
      </NuxtLink>
    </div>

    <!-- Fitur Dashboard -->
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-4">
      <NuxtLink to="/produk-laris" class="p-4 border rounded shadow hover:bg-green-50 text-center font-medium">
        🔍 Cari Produk Laris Shopee
      </NuxtLink>
      <NuxtLink to="/produk-saya" class="p-4 border rounded shadow hover:bg-green-50 text-center font-medium">
        📦 Lihat Produk Tersimpan
      </NuxtLink>
      <NuxtLink to="/pengaturan" class="p-4 border rounded shadow hover:bg-green-50 text-center font-medium">
        ⚙️ Pengaturan
      </NuxtLink>
    </div>
  </div>
</template>

<script setup>
</script>
