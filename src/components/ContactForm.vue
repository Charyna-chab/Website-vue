<template>
  <div class="max-w-3xl mx-auto px-6 py-10 bg-white rounded-3xl shadow-lg flex flex-col md:flex-row items-center gap-10 mt-6 mb-6">
    <!-- Contact Form -->
    <div class="w-full md:w-1/2">
      <h2 class="text-3xl font-extrabold text-gray-800 mb-6">Get in Touch</h2>
      <form @submit.prevent="submitForm" class="space-y-6">
        <div>
          <label class="block text-base font-medium text-gray-700 mb-2">Name</label>
          <input
            v-model="form.name"
            type="text"
            class="w-full border border-green-400 rounded-lg p-3 text-base focus:ring-2 focus:ring-green-500 focus:outline-none"
            required
          />
        </div>

        <div>
          <label class="block text-base font-medium text-gray-700 mb-2">Email</label>
          <input
            v-model="form.email"
            type="email"
            class="w-full border border-green-400 rounded-lg p-3 text-base focus:ring-2 focus:ring-green-500 focus:outline-none"
            required
          />
        </div>

        <div>
          <label class="block text-base font-medium text-gray-700 mb-2">Message</label>
          <textarea
            v-model="form.message"
            rows="5"
            class="w-full border border-green-400 rounded-lg p-3 text-base focus:ring-2 focus:ring-green-500 focus:outline-none"
            required
          ></textarea>
        </div>

        <button
          type="submit"
          class="bg-green-600 text-white px-6 py-3 rounded-lg text-base font-semibold hover:bg-green-700 transition"
        >
          Send Message
        </button>
      </form>
    </div>

    <!-- Image -->
    <div class="w-full md:w-1/2">
      <img
        src="https://i.pinimg.com/736x/88/43/05/884305d040320f7adca73b9439e87e18.jpg"
        alt="Contact Illustration"
        class="rounded-2xl shadow-md w-full h-auto object-cover"
      />
    </div>
  </div>
</template>

<script setup>
import { reactive } from 'vue'

const form = reactive({
  name: '',
  email: '',
  message: ''
})

function submitForm() {
  alert(`Thank you, ${form.name}! We have received your message.`)
  form.name = ''
  form.email = ''
  form.message = ''
}
</script>
