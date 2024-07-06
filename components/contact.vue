<!-- components/ContactUs.vue -->
<template>
  <v-container class="my-36">
    <div class="flex flex-col items-center justify-center p-6">
      <div class="flex flex-col mx-auto mb-12">
        <h1 class="text-h3 text-black text-center font-bold mb-4">
          Contact Us
        </h1>
        <p class="text-center mb-6 text-gray-800 text-xl">
          Most calendars are designed for teams. <br />
          Slate is designed for freelancers.
        </p>
      </div>

      <div class="flex gap-7">
        <div
          class="flex flex-col lg:flex-row items-start lg:items-center bg-white p-6 rounded-lg shadow-2xl"
        >
          <div class="w-full mb-6">
            <h2 class="text-lg font-bold mb-4">Contact Us</h2>
            <form class="space-y-4" @submit.prevent="submitForm">
              <v-text-field
                v-model="formData.name"
                label="Your Name"
                outlined
                rounded="lg"
                dense
              ></v-text-field>
              <v-text-field
                v-model="formData.email"
                label="Your Email"
                outlined
                rounded="lg"
                dense
              ></v-text-field>
              <v-textarea
                v-model="formData.message"
                label="Your Message"
                outlined
                dense
              ></v-textarea>
              <v-btn
                color="primary"
                block
                class="mt-3 w-fit"
                width="fit"
                type="submit"
              >
                <span> Send </span>
              </v-btn>
            </form>
          </div>
        </div>

        <div>
          <div class="w-full">
            <div class="flex gap-4">
              <div class="mb-4 flex gap-2 flex-col">
                <v-icon color="#2091f9" class="mr-2"
                  >mdi-map-marker-outline</v-icon
                >
                <p class="text-center">
                  6386 Spring St undefined Anchorage,<br />
                  Georgia 12473 United States
                </p>
              </div>
              <div class="mb-4 gap-3 flex flex-col items-center">
                <v-icon color="#2091f9" class="mr-2">mdi-cellphone</v-icon>
                <p class="text-center">(843) 555-0130</p>
              </div>
              <div class="mb-4 gap-3 flex flex-col items-center">
                <v-icon color="#2091f9" class="mr-2">mdi-email-outline</v-icon>
                <p class="text-center">willie.jennings@example.com</p>
              </div>
            </div>
            <div>
              <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3733.9861668232176!2d-84.56051978511258!3d33.85822858065627!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x88f59eafd7c84435%3A0xe42b521b32e2d96e!2s6386%20Spring%20St%20undefined%2C%20Anchorage%2C%20GA%2012473%2C%20USA!5e0!3m2!1sen!2sus!4v1625554740537!5m2!1sen!2sus"
                width="100%"
                height="450"
                style="border: 0"
                allowfullscreen=""
                loading="lazy"
                referrerpolicy="no-referrer-when-downgrade"
              ></iframe>
            </div>
          </div>

          <div class="mt-6 flex space-x-4">
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
        </div>
      </div>
    </div>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      formData: {
        name: '',
        email: '',
        message: '',
      },
    }
  },
  methods: {
    submitForm() {
      // Handle form submission logic here
      console.log('Form submitted with data:', this.formData)
    },
  },
}
</script>

<style scoped>
/* Add any scoped styles if necessary */
</style>
