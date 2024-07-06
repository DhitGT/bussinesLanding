<template>
  <div class="container mx-auto p-6">
    <h1 class="text-4xl font-bold text-center mb-4">Features</h1>
    <p class="text-lg text-center mb-8">
      Most calendars are designed for teams. Slate is designed for freelancers
    </p>
    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
      <div class="rounded-lg shadow-md p-6 bg-white">
        <div class="flex items-center mb-4">
          <v-icon class="mdi mdi-font-bold text-blue-500"
            >mdi-format-font</v-icon
          >
          <h2 class="ml-4 font-bold">OpenType features</h2>
        </div>
        <p>
          Slate helps you see how many more days you need to work to reach your
          financial goal.
        </p>
      </div>
      <div class="rounded-lg shadow-md p-6 bg-white">
        <div class="flex items-center mb-4">
          <v-icon class="mdi mdi-chart-bar text-blue-500">mdi-chart-bar</v-icon>
          <h2 class="ml-4 font-bold">Design with real data</h2>
        </div>
        <p>
          Slate helps you see how many more days you need to work to reach your
          financial goal.
        </p>
      </div>
      <div class="rounded-lg shadow-md p-6 bg-white">
        <div class="flex items-center mb-4">
          <v-icon class="mdi mdi-rocket text-blue-500">mdi-rocket</v-icon>
          <h2 class="ml-4 font-bold">Fastest way to take action</h2>
        </div>
        <p>
          Slate helps you see how many more days you need to work to reach your
          financial goal.
        </p>
      </div>
    </div>
    <div class="mt-16">
      <div class="relative w-full h-0 pb-[56.25%]">
        <iframe
          class="absolute top-0 left-0 w-full h-full rounded-lg shadow-md"
          src="https://www.youtube.com/embed/1drDHQRvAb0"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Features',
}
</script>
