<script setup>
import { ref } from 'vue'
import VDialog from './components/VDialog.vue'

const show = ref(false)
</script>
<template>
  <div class="flex h-screen w-screen items-center justify-center bg-gray-900">
    <div class="min-h-[300px] min-w-[500px] rounded bg-white p-5 text-center">
      <div class="flex h-[300px] w-full flex-col items-center justify-center">
        <button @click="show = true" class="bg-teal-500 p-2 text-white">Show dialog</button>
        <v-dialog v-model="show"> Hello word </v-dialog>
      </div>
    </div>
  </div>
</template>
