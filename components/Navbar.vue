<template>
  <nav
    :class="{ 'bg-gray-900': !isTopScroll, 'bg-transparent': isTopScroll }"
    class="shadow"
  >
    <!-- navbar -->
    <div
      class="container mx-auto px-4 py-2 gap-4 flex justify-between items-center"
    >
      <div class="hidden md:flex items-center space-x-4">
        <a href="/" class="text-gray-500 hover:text-gray-700">Home</a>
        <a href="/" class="text-gray-500 hover:text-gray-700">Product</a>
        <a href="/" class="text-gray-500 hover:text-gray-700">Pricing</a>
        <a href="/" class="text-gray-500 hover:text-gray-700">About</a>
        <a href="/" class="text-gray-500 hover:text-gray-700">Contact</a>
      </div>
      <div class="flex items-center">
        <a href="/" class="text-xl font-bold text-gray-800">FIGMA LAND</a>
      </div>
      <div class="flex gap-4 justify-end md:hidden">
        <button
          @click="toggleMobileMenu"
          class="text-gray-500 hover:text-gray-700 focus:outline-none"
        >
          <v-icon color="white">mdi-menu</v-icon>
          <!-- DSFSDFSDFSDFSDF -->
        </button>
      </div>
      <div class="hidden md:flex gap-4 justify-end">
        <a href="#" class="text-blue-500 hover:text-blue-700"
          ><v-icon color="#fff">mdi-twitter</v-icon></a
        >
        <a href="#" class="text-blue-500 hover:text-blue-700"
          ><v-icon color="#fff">mdi-facebook</v-icon></a
        >
        <a href="#" class="text-blue-500 hover:text-blue-700"
          ><v-icon color="#fff">mdi-linkedin</v-icon></a
        >
      </div>
    </div>

    <!-- Mobile Menu -->
    <div v-if="isMobileMenuOpen" class="md:hidden bg-gray-900">
      <a href="/" class="block py-2 px-4 text-gray-100 hover:text-white"
        >Home</a
      >
      <a href="/" class="block py-2 px-4 text-gray-100 hover:text-white"
        >Product</a
      >
      <a href="/" class="block py-2 px-4 text-gray-100 hover:text-white"
        >Pricing</a
      >
      <a href="/" class="block py-2 px-4 text-gray-100 hover:text-white"
        >About</a
      >
      <a href="/" class="block py-2 px-4 text-gray-100 hover:text-white"
        >Contact</a
      >
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',

  data() {
    return {
      isTopScroll: true,
      isMobileMenuOpen: false,
    }
  },

  mounted() {
    window.addEventListener('scroll', this.handleScroll)
  },

  beforeDestroy() {
    window.removeEventListener('scroll', this.handleScroll)
  },

  methods: {
    handleScroll() {
      this.isTopScroll = window.scrollY === 0
    },

    toggleMobileMenu() {
      this.isMobileMenuOpen = !this.isMobileMenuOpen
    },
  },
}
</script>

<style scoped>
nav {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1;
  transition: background-color 0.3s ease;
}

nav a:visited {
  text-decoration: none;
  color: rgb(222, 222, 222); /* Set the color to a darker gray */
}

nav a {
  text-decoration: none;
}

/* Styling for mobile menu button */
button {
  color: inherit;
  cursor: pointer;
}

/* Styling for mobile menu links */
div.md:hidden a {
  display: block;
  padding: 10px;
}

/* Hide mobile menu initially */
div.md:hidden {
  display: none;
}
</style>
