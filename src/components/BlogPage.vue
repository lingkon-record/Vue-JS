<template>
  <div class="min-h-screen bg-gray-100">
    <!-- Header Section -->
    <header class="bg-white shadow">
      <div class="max-w-7xl mx-auto py-6 px-4 sm:px-6 lg:px-8">
        <h1 class="text-3xl font-bold text-gray-900">My Blog</h1>
      </div>
    </header>

    <!-- Main Content Section -->
    <main class="max-w-7xl mx-auto py-6 sm:px-6 lg:px-8">
      <!-- Featured Blog Section -->
      <section class="mb-8">
        <div class="max-w-4xl mx-auto bg-white rounded-lg overflow-hidden shadow-lg">
          <img src="https://www.pranfoods.net/sites/default/files/2023-08/COMMON%20BANNER.jpeg" alt="Featured Blog" class="w-full h-64 object-cover object-center">
          <div class="p-6">
            <h2 class="text-2xl font-bold mb-2">Featured Blog Post</h2>
            <p class="text-gray-700">
              Our Brands | Pran Foods
            </p>
            <a href="#" class="text-blue-600 hover:underline mt-2 inline-block">Read more...</a>
          </div>
        </div>
      </section>

      <!-- Latest Posts Section -->
      <section class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6">
        <div v-for="post in latestPosts" :key="post.id" class="bg-white rounded-lg overflow-hidden shadow-md">
          <img :src="post.image" alt="Latest Post" class="w-full h-48 object-cover object-center">
          <div class="p-4">
            <h3 class="text-lg font-bold mb-2">{{ post.title }}</h3>
            <p class="text-gray-700">{{ post.excerpt }}</p>
            <a href="#" class="text-blue-600 hover:underline mt-2 inline-block">Read more...</a>
          </div>
        </div>
      </section>
    </main>

    <!-- Footer Section -->
    <footer class="bg-white shadow mt-6">
      <div class="max-w-7xl mx-auto py-4 px-4 sm:px-6 lg:px-8">
        <p class="text-gray-500 text-center">&copy; 2024 My Blog. All rights reserved.</p>
      </div>
    </footer>
  </div>
</template>

<script>
export default {
  name: 'BlogPage',
  data() {
    return {
      latestPosts: [
        { id: 2, image: 'https://mir-s3-cdn-cf.behance.net/projects/404/d0e7cd199150183.Y3JvcCwxNTM0LDEyMDAsMzQsMA.png', title: 'Post 2', excerpt: 'Suspendisse varius enim in eros elementum tristique.' },
        { id: 1, image: 'https://www.retailerbd.com/wp-content/uploads/2023/10/PRAN-Mr.-Noodles-Magic-Masala-Paper-Cup-35gm.jpg', title: 'Post 1', excerpt: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.' },
        { id: 3, image: 'https://m.media-amazon.com/images/I/51Sin2bDq8L._AC_UF1000,1000_QL80_.jpg', title: 'Post 3', excerpt: 'Ut enim ad minim veniam, quis nostrud exercitation ullamco.' },
      ],
    };
  },
};
</script>

<style scoped>
/* Scoped styles can be added here if necessary */
</style>
