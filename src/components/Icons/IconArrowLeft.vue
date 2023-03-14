<script setup>
defineProps({
  class: {
    type: String,
    requared: true
  }
})
</script>

<template>
  <svg :class="class" width="30" height="25" viewBox="0 0 30 25" fill='none' xmlns="http://www.w3.org/2000/svg">
    <path
      d="M14.2969 19.5312L5.85938 12.5L14.2969 5.46875M7.03125 12.5H24.1406"
      fill="none"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
  </svg>
</template>
