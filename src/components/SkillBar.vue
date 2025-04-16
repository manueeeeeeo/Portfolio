<template>
    <div>
      <div class="flex justify-between text-sm mb-1">
        <span>{{ name }}</span>
        <span>{{ level }}%</span>
      </div>
      <div class="w-full bg-gray-200 rounded-full h-3">
        <div
          class="bg-blue-500 h-3 rounded-full transition-all duration-500"
          :style="{ width: level + '%' }"
        ></div>
      </div>
    </div>
  </template>
  
  <script setup>
  defineProps({
    name: String,
    level: Number
  })
  </script>
  