<template>
  <v-container class="my-24">
    <v-row class="justify-center">
      <v-col cols="12" md="12" class="w-full">
        <h1 class="text-h3 text-center font-bold mb-4">Partners</h1>
        <p class="text-center mb-6 text-xl">
          Most calendars are designed for teams. <br />
          Slate is designed for freelancers.
        </p>

        <v-row class="mb-4 w-100">
          <v-col
            cols="12"
            md="3"
            v-for="(partner, index) in partners"
            :key="index"
            class="p-0 flex gap-0"
          >
            <v-card
              tile
              class="flex m-0 items-center justify-center border border-gray-300 w-full aspect-w-1 aspect-h-1"
            >
              <v-card-text
                class="flex items-center justify-center w-full h-full"
              >
                <img
                  :src="partner.logo"
                  :alt="partner.name"
                  class="max-w-3/4 max-h-3/4"
                />
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>

        <div class="flex justify-center">
          <v-btn
            color="primary"
            rounded="xl"
            class="py-6 px-10"
            style="width: fit-content"
          >
            Try For Free
          </v-btn>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      partners: [
        {
          name: 'Google',
          logo: 'https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png',
        },
        {
          name: 'Amazon',
          logo: 'https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/Amazon_logo.svg/1200px-Amazon_logo.svg.png',
        },
        {
          name: 'Microsoft',
          logo: 'https://upload.wikimedia.org/wikipedia/commons/thumb/9/96/Microsoft_logo_%282012%29.svg/250px-Microsoft_logo_%282012%29.svg.png',
        },
        {
          name: 'Uber',
          logo: 'https://upload.wikimedia.org/wikipedia/commons/thumb/5/58/Uber_logo_2018.svg/220px-Uber_logo_2018.svg.png',
        },
        {
          name: 'Dropbox',
          logo: 'https://upload.wikimedia.org/wikipedia/commons/thumb/c/cb/Dropbox_logo_2017.svg/220px-Dropbox_logo_2017.svg.png',
        },

        {
          name: 'Uber',
          logo: 'https://upload.wikimedia.org/wikipedia/commons/thumb/5/58/Uber_logo_2018.svg/220px-Uber_logo_2018.svg.png',
        },
        {
          name: 'Google',
          logo: 'https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png',
        },
        {
          name: 'Amazon',
          logo: 'https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/Amazon_logo.svg/1200px-Amazon_logo.svg.png',
        },
      ],
    }
  },
}
</script>

<style scoped>
.v-card {
  border-radius: 10px;
  padding: 16px;
}
</style>
