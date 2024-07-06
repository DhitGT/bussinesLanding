<template>
  <div class="jumbotron relative pt-28 h-screen">
    <div class="bg-image absolute top-0 left-0 w-full h-full">
      <div
        class="overlay absolute top-0 left-0 w-full h-full bg-black opacity-50"
      ></div>
    </div>
    <div class="triangle-separator absolute bottom-0 left-0 w-full h-64">
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1440 320"
        preserveAspectRatio="none"
      >
        <path
          fill="#ffffff"
          d="M0,32L720,260L1440,96L1540,320L720,320L0,320Z"
        ></path>
      </svg>
    </div>
    <div
      class="container relative flex flex-col items-center justify-center h-[70%] mx-auto px-4 sm:px-6 lg:px-8"
    >
      <div class="text-center w-[100] mx-auto">
        <h1
          class="text-4xl font-bold tracking-tight text-gray-100 sm:text-5xl md:text-6xl"
        >
          The best products start with Figma
        </h1>
        <p
          class="mt-3 text-base text-gray-200 sm:mt-4 sm:text-lg md:mt-5 md:text-xl"
        >
          Most calendars are designed for teams. Slate is designed for
          freelancers.
        </p>
        <div class="mt-6">
          <button
            type="button"
            class="inline-flex items-center px-4 py-2 border border-transparent text-sm font-medium rounded-md shadow-sm text-white bg-[#2091f9] hover:bg-[#1041f9]focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500"
          >
            Try For Free
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.jumbotron {
  height: 100vh;
  background-image: url('https://images.unsplash.com/photo-1516321497487-e288fb19713f?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D');
  background-size: cover;
  background-position: center;
}

.overlay {
  background-color: #000;
  opacity: 0.5;
}

.triangle-separator {
}

.triangle-separator svg {
  width: 100%;
  height: 100%;
}
</style>
