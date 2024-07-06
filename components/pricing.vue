<template>
  <div class="bg-[#252b42] py-12">
    <v-container fill-height>
      <div class="flex flex-col mx-auto mb-12">
        <h1 class="text-h3 text-white text-center font-bold mb-4">Pricing</h1>
        <p class="text-center mb-6 text-white text-xl">
          Most calendars are designed for teams. <br />
          Slate is designed for freelancers.
        </p>
      </div>
      <v-row align="center" justify="center" class="md:px-36 bg-[#252b42]">
        <v-col
          v-for="(item, index) in pricingItems"
          :key="index"
          cols="12"
          md="4"
          class="pa-5 flex flex-col items-center justify-center"
        >
          <div
            :class="[
              index === 1 ? 'middle-card' : 'bg-white',
              index === 1 ? 'h-[40em]' : 'h-[30em]',
            ]"
            class="pa-3 w-fit rounded-lg flex justify-around items-center"
          >
            <div
              class="flex-grow flex flex-col my-auto justify-center items-center"
            >
              <div class="text-h5 text-center mb-3">{{ item.title }}</div>
              <div class="text-center">
                {{ item.description }}
              </div>
              <div class="text-h3 text-center mt-3 font-weight-bold">
                {{ item.price }}<span class="text-subtitle-1">$</span>
              </div>
              <div class="text-center text-subtitle-1">Per Month</div>
              <div class="mt-3 text-center">
                <div
                  v-for="(feature, featureIndex) in item.features"
                  :key="featureIndex"
                  class="mb-2"
                >
                  {{ feature }}
                </div>
              </div>
              <v-btn
                :color="index === 1 ? 'white' : 'primary'"
                block
                class="mt-3"
              >
                <span :class="index === 1 ? 'text-[#2091f9]' : ''">
                  Order Now
                </span>
              </v-btn>
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      pricingItems: [
        {
          title: 'FREE',
          description: 'Organize across all apps by hand',
          price: 0,
          features: [
            'Pricing Feature',
            'Pricing Feature',
            'Pricing Feature',
            'Pricing Feature',
            'Pricing Feature',
          ],
        },
        {
          title: 'STANDARD',
          description: 'Organize across all apps by hand',
          price: 10,
          features: [
            'Pricing Feature',
            'Pricing Feature',
            'Pricing Feature',
            'Pricing Feature',
            'Pricing Feature',
          ],
        },
        {
          title: 'BUSINESS',
          description: 'Organize across all apps by hand',
          price: 99,
          features: [
            'Pricing Feature',
            'Pricing Feature',
            'Pricing Feature',
            'Pricing Feature',
            'Pricing Feature',
          ],
        },
      ],
    }
  },
}
</script>

<style scoped>
.v-card {
  background-color: #f0f0f0;
  border-radius: 10px;
  box-shadow: none;
}

.v-card:hover {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.v-btn {
  background-color: #007bff;
  color: #fff;
  border-radius: 10px;
}

.v-btn:hover {
  opacity: 0.8;
}

.middle-card {
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
  background-color: #2091f9;
  color: white;
}

.red {
  background-color: red;
}

.green {
  background-color: #28a745; /* Adjusted to match Tailwind green shade */
  color: white;
}
</style>
