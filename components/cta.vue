<template>
  <div class="container mx-auto flex items-center py-12 justify-between">
    <img src="newsletter.png" class="h-[30em]" alt="" />
    <div>
      <p class="text-gray-600 font-semi-bold">At your fingertips</p>
      <h1 class="text-4xl my-4 font-light text-gray-900">
        Lightning fast <br />
        prototyping
      </h1>
      <span class="text-gray-600">
        <span class="font-bold"> Subscribe to our Newsletter </span>

        <br />
        Available exclusively on Figmaland</span
      >
      <div class="flex items-center mt-4">
        <input
          type="email"
          placeholder="Your Email"
          class="px-4 py-2 rounded-md border border-gray-300 focus:outline-none focus:ring-2 focus:ring-blue-500"
        />
        <button
          class="ml-4 px-6 py-2 rounded-md bg-blue-500 text-white hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-500"
        >
          Subscribe
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
}
</script>
