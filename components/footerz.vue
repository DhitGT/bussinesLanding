<template>
  <footer class="bg-gray-800 text-gray-400 py-10">
    <div class="container mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
        <div class="text-left">
          <h3 class="font-bold text-xl">Pages</h3>
          <ul>
            <li class="py-2">
              <a href="#">Home</a>
            </li>
            <li class="py-2">
              <a href="#">Product</a>
            </li>
            <li class="py-2">
              <a href="#">Pricing</a>
            </li>
            <li class="py-2">
              <a href="#">About</a>
            </li>
            <li class="py-2">
              <a href="#">Contact</a>
            </li>
          </ul>
        </div>
        <div class="text-left">
          <h3 class="font-bold text-xl">Tomothy</h3>
          <ul>
            <li class="py-2">Eleanor Edwards</li>
            <li class="py-2">Ted Robertson</li>
            <li class="py-2">Annette Russell</li>
            <li class="py-2">Jennie Mckinney</li>
            <li class="py-2">Gloria Richards</li>
          </ul>
        </div>
        <div class="text-left">
          <h3 class="font-bold text-xl">Jane Black</h3>
          <ul>
            <li class="py-2">Eleanor Edwards</li>
            <li class="py-2">Ted Robertson</li>
            <li class="py-2">Annette Russell</li>
            <li class="py-2">Jennie Mckinney</li>
            <li class="py-2">Gloria Richards</li>
          </ul>
        </div>
        <div class="text-left">
          <h3 class="font-bold text-xl">Contact Us</h3>
          <ul>
            <li class="py-2">
              <v-icon color="#2091f9" size="18" class="mr-2"
                >mdi-map-marker</v-icon
              >
              6386 Spring St undefined Anchorage
            </li>
            <li class="py-2">
              <v-icon color="#2091f9" size="18" class="mr-2">mdi-phone</v-icon>
              (239) 555-0108
            </li>
            <li class="py-2">
              <div class="flex space-x-4">
                <a href="#" class="text-blue-500 hover:text-blue-700"
                  ><v-icon color="#2091f9">mdi-twitter</v-icon></a
                >
                <a href="#" class="text-blue-500 hover:text-blue-700"
                  ><v-icon color="#2091f9">mdi-facebook</v-icon></a
                >
                <a href="#" class="text-blue-500 hover:text-blue-700"
                  ><v-icon color="#2091f9">mdi-linkedin</v-icon></a
                >
              </div>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'Footer',
}
</script>

<style scoped>
</style>
