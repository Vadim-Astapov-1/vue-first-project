<script setup>
defineProps({
  class: {
    type: String,
    requared: true
  }
})
</script>

<template>
  <svg :class="class" width="24" height="24" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
    <path
      d="M11 18.6667H13V13H18.6667V11H13V5.33333H11V11H5.33333V13H11V18.6667ZM2 24C1.46667 24 1 23.8 0.6 23.4C0.2 23 0 22.5333 0 22V2C0 1.46667 0.2 1 0.6 0.6C1 0.2 1.46667 0 2 0H22C22.5333 0 23 0.2 23.4 0.6C23.8 1 24 1.46667 24 2V22C24 22.5333 23.8 23 23.4 23.4C23 23.8 22.5333 24 22 24H2ZM2 22H22V2H2V22Z"
    />
  </svg>
</template>
