<script setup>
defineProps({
  class: {
    type: String,
    requared: true
  }
})
</script>

<template>
  <svg :class="class" width="19" height="22" viewBox="0 0 19 22" xmlns="http://www.w3.org/2000/svg">
    <g filter="url(#filter0_d_116_7)">
      <path
        d="M5.28125 7.14844L9.5 2.92969L13.7188 7.14844M9.5 3.51562V12.0703"
        stroke="#FF0000"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round"
      />
    </g>
    <defs>
      <filter
        id="filter0_d_116_7"
        x="-2"
        y="0"
        width="23"
        height="23"
        filterUnits="userSpaceOnUse"
        color-interpolation-filters="sRGB"
      >
        <feFlood flood-opacity="0" result="BackgroundImageFix" />
        <feColorMatrix
          in="SourceAlpha"
          type="matrix"
          values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"
          result="hardAlpha"
        />
        <feOffset dy="4" />
        <feGaussianBlur stdDeviation="2" />
        <feComposite in2="hardAlpha" operator="out" />
        <feColorMatrix type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0.25 0" />
        <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow_116_7" />
        <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow_116_7" result="shape" />
      </filter>
    </defs>
  </svg>
</template>
