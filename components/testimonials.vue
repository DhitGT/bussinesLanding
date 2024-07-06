<template>
  <v-container class="my-24">
    <v-row class="justify-center">
      <v-col cols="12" md="8">
        <h1 class="text-h3 text-center font-bold mb-4">Testimonials</h1>
        <v-row class="justify-center">
          <v-col cols="12" md="4">
            <v-card flat class="d-flex align-center justify-center">
              <v-card-text>
                <img src="ibm.png" alt="IBM" class="w-100" />
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
        <p class="text-center mb-6">
          Most calendars are designed for teams. Slate is designed for
          <br />
          freelancers who want a simple way to plan their schedule.
        </p>
        <v-row class="justify-center">
          <v-card flat class="d-flex align-center justify-center">
            <div class="flex gap-2">
              <v-avatar>
                <img src="https://placehold.co/200" alt="" />
              </v-avatar>
              <div>
                <span class="text-center text-sm">Jhon Doe Samuels</span>
                <br />
                <span class="text-center text-xs">Ui designer</span>
              </div>
            </div>
          </v-card>
        </v-row>

        <div class="flex justify-center mt-6">
          <v-btn
            color="primary"
            rounded="xl"
            class="py-6 px-10"
            style="width: fit-content"
          >
            More Testimonials
          </v-btn>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  head() {
    return {
      title: 'Testimonials',
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
