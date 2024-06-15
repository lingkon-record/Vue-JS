<template>
  <div class="bg-gray-100 mt-6 min-h-screen flex items-center justify-center">
    <div class="max-w-4xl bg-white p-8 rounded shadow-lg">
      <h2 class="text-3xl font-bold mb-6 text-center">Welcome to - প্রাণ ঝাল চানাচুর</h2>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
        <div v-for="(product, index) in products" :key="index" class="bg-gray-200 p-6 rounded shadow-md">
          <h3 class="text-xl font-semibold mb-2">{{ product.name }}</h3>
          <p class="text-gray-700 mb-4">{{ product.description }}</p>
          <!-- <p class="text-gray-800 font-bold">${{ product.price }}</p> -->
        </div>
      </div>
      <div class="flex justify-center mt-6">
        <button class="bg-blue-500 hover:bg-blue-600 text-white font-bold py-2 px-4 rounded">
          View More
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BannerAdd',
  data() {
    return {
      products: [
        { name: 'চানাচুর', description: 'চানাচুর একপ্রকার ভাজা নাশতা জাতীয় হালকা খাবার। ', price: 12.99 },
        { name: 'ডালমুঠ। ছোলা', description: 'প্রায়শই চিনাবাদাম, চিঁড়া, সবুজাভ ভাজা মটরশুটিঁ ইত্যাদি যোগ করা হয়', price: 19.99 },
        { name: 'হালকা খাবার', description: 'এটি মূলত ছোলা বা অড়হড় ডালের মিহি গুঁড়া (বেসন) থেকে তৈরি হয়।', price: 14.99 },
      ]
    };
  }
};
</script>

<style scoped>
/* No additional styles needed as Tailwind CSS classes are used inline */
</style>
