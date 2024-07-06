<template>
  <div class="hero h-[fit] my-24 bg-white">
    <div class="container flex mx-auto p-6 gap-2">
      <div class="flex flex-col h-100 justify-evenly">
        <div>
          <h1 class="text-4xl font-bold text-start mb-4">
            Fastest way to organize
          </h1>
        </div>
        <div>
          <p class="text-2xl text-start mb-8">
            Most calendars are designed for teams. <br />
            Slate is designed for freelancers
          </p>
        </div>
        <div class="flex justify-start max-h-[40px]">
          <v-btn
            class="bg-orange-500 hover:bg-orange-700 text-white text-xl font-bold p-6 rounded-xl"
            @click="tryForFree"
            rounded="xl"
            color="#2091f9"
          >
            <span class="text-white"> Try For Free </span>
            <v-icon
              class="mdi mdi-arrow-right text-white text-xl ml-2"
              color="white"
              >mdi-arrow-right</v-icon
            >
          </v-btn>
        </div>
      </div>
      <img
        src="laptop.png"
        class="max-w-[60em] max-h-[20em] rounded-lg"
        alt="Slate Calendar Screenshot"
      />
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    tryForFree() {
      // Handle try for free button click
    },
  },
}
</script>

<style scoped>
.hero {
  @apply bg-white;
}

.container {
  @apply mx-auto p-6;
}
</style>
