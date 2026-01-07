<template>
  <div class="min-h-screen bg-gradient-to-br from-blue-50 to-indigo-100 flex items-center justify-center p-4">
    <div class="max-w-2xl w-full">
      <div class="bg-white rounded-2xl shadow-xl p-8 md:p-12 text-center">
        <!-- Logo/Icon -->
        <div class="mb-6">
          <div class="inline-flex items-center justify-center w-20 h-20 bg-indigo-600 rounded-full mb-4">
            <svg class="w-12 h-12 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path>
            </svg>
          </div>
        </div>

        <!-- Welcome Heading -->
        <h1 class="text-4xl md:text-5xl font-bold text-gray-900 mb-4">
          Welcome to Vue.js
        </h1>
        
        <p class="text-xl text-gray-600 mb-8">
          Your project is ready with Tailwind CSS
        </p>

        <!-- Features Grid -->
        <div class="grid grid-cols-1 md:grid-cols-3 gap-4 mb-8">
          <div class="p-4 bg-indigo-50 rounded-lg">
            <div class="text-2xl mb-2">⚡</div>
            <h3 class="font-semibold text-gray-900 mb-1">Vite</h3>
            <p class="text-sm text-gray-600">Lightning fast build tool</p>
          </div>
          <div class="p-4 bg-indigo-50 rounded-lg">
            <div class="text-2xl mb-2">🎨</div>
            <h3 class="font-semibold text-gray-900 mb-1">Tailwind</h3>
            <p class="text-sm text-gray-600">Utility-first CSS</p>
          </div>
          <div class="p-4 bg-indigo-50 rounded-lg">
            <div class="text-2xl mb-2">🚀</div>
            <h3 class="font-semibold text-gray-900 mb-1">Vue 3</h3>
            <p class="text-sm text-gray-600">Progressive framework</p>
          </div>
        </div>

        <!-- Action Buttons -->
        <div class="flex flex-col sm:flex-row gap-4 justify-center">
          <a
            href="https://vuejs.org"
            target="_blank"
            rel="noopener noreferrer"
            class="px-6 py-3 bg-indigo-600 text-white rounded-lg font-semibold hover:bg-indigo-700 transition-colors duration-200"
          >
            Vue Docs
          </a>
          <a
            href="https://tailwindcss.com"
            target="_blank"
            rel="noopener noreferrer"
            class="px-6 py-3 bg-gray-200 text-gray-800 rounded-lg font-semibold hover:bg-gray-300 transition-colors duration-200"
          >
            Tailwind Docs
          </a>
        </div>

        <!-- Counter Demo -->
        <div class="mt-8 pt-8 border-t border-gray-200">
          <p class="text-gray-600 mb-4">Quick demo:</p>
          <div class="flex items-center justify-center gap-4">
            <button
              @click="decrement"
              class="px-4 py-2 bg-red-500 text-white rounded-lg hover:bg-red-600 transition-colors"
            >
              −
            </button>
            <span class="text-3xl font-bold text-gray-900 min-w-[60px]">{{ count }}</span>
            <button
              @click="increment"
              class="px-4 py-2 bg-green-500 text-white rounded-lg hover:bg-green-600 transition-colors"
            >
              +
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const count = ref(0)

const increment = () => {
  count.value++
}

const decrement = () => {
  count.value--
}
</script>
