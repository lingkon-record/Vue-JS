<template >
    <div class="max-w-7xl mt-20 mx-auto p-4">
      <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-6">
        <div v-for="product in products" :key="product.id" class="bg-white shadow-lime-500 shadow-md rounded-lg overflow-hidden">
          <img :src="product.image" alt="Product Image" class="w-full mt-2 h-56 object-cover object-center">
          <div class="p-4">
            <h2 class="text-lg font-bold">{{ product.title }}</h2>
            <p class="text-gray-700">{{ product.price }}</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    name: 'ProductGrid',
    data() {
      return {
        products: [
          { id: 1, image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQbXsZVn7D8mjdNebwMm9lV03sPevTjo6e_Yg&s', title: ' চানাচুর 1', price: '$20.00' },
          { id: 2, image: 'https://multi.wellbd.com/images/jhal-chanachur.png', title: ' চানাচুর 2', price: '$25.00' },
          { id: 3, image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQbXsZVn7D8mjdNebwMm9lV03sPevTjo6e_Yg&s', title: ' চানাচুর 3', price: '$30.00' },
          { id: 4, image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQW-QO-P0pdwpvJtpcCR5EQNOWF1JcnVdhI-z6BG3kZPswylVvPgtNNXD7NbZUFZNkl3NY&usqp=CAU', title: ' চানাচুর 4', price: '$35.00' },
          { id: 5, image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQbXsZVn7D8mjdNebwMm9lV03sPevTjo6e_Yg&s', title: 'Product 5', price: '$40.00' },
          { id: 6, image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS8iGSFLn8keMi8xoFRFYMoWLh3xH8Mhy89RK0p-qSIpDnM5jOafmyDtzFAXEmkXO4cIhQ&usqp=CAU', title: ' চানাচুর 6', price: '$45.00' },
          { id: 7, image: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQbXsZVn7D8mjdNebwMm9lV03sPevTjo6e_Yg&s', title: ' চানাচুর 7', price: '$50.00' },
          { id: 8, image: 'https://multi.wellbd.com/images/jhal-chanachur.png', title: ' চানাচুর 8', price: '$55.00' },
        ],
      };
    },
  };
  </script>
  
  <style scoped>
  /* You can add scoped styles here if necessary */
  </style>
  