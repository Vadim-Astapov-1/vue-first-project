<script setup>
defineProps({
  class: {
    type: String,
    requared: true
  }
})
</script>

<template>
  <svg :class="class" width="25" height="25" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg">
    <path
      d="M17.9688 17.9688L7.03125 7.03125M17.9688 7.03125L7.03125 17.9688"
      stroke="black"
      stroke-linecap="round"
      stroke-linejoin="round"
    />
  </svg>
</template>
