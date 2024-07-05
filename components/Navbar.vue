<template>
  <nav class="shadow transparent">
    <!-- navbar -->
    <div class="container mx-auto px-4 py-2 flex justify-between items-center">
      <div class="flex items-center">
        <a href="/" class="text-xl font-bold text-gray-800"> FIGMA LAND </a>
      </div>
      <div class="hidden md:flex items-center space-x-4">
        <a href="/" class="text-gray-500 hover:text-gray-700">Home</a>
        <a href="/" class="text-gray-500 hover:text-gray-700">Product</a>
        <a href="/" class="text-gray-500 hover:text-gray-700">Pricing</a>
        <a href="/" class="text-gray-500 hover:text-gray-700">About</a>
        <a href="/" class="text-gray-500 hover:text-gray-700">Contact</a>
      </div>
      <div class="flex items-center space-x-4">
        <a href="/" class="text-gray-500 hover:text-gray-700">
          <i class="fab fa-twitter"></i>
        </a>
        <a href="/" class="text-gray-500 hover:text-gray-700">
          <i class="fab fa-facebook"></i>
        </a>
        <a href="/" class="text-gray-500 hover:text-gray-700">
          <i class="fab fa-linkedin-in"></i>
        </a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style scoped>
nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1;
  background-color: #fff; /* Add a background color to the navbar */
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1); /* Add a box shadow to the navbar */
}

nav a:visited {
  text-decoration: none;
  color: rgb(222, 222, 222); /* Set the color to a darker gray */
}
</style>
