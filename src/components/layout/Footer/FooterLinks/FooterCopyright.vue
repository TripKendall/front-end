<template>
  <p class="mt-8 text-xs text-gray-500 md:mt-0 md:order-1 py-2">
    &copy; {{ info.year }}
    <a class="primaryText hover:text-sky-600" :href="info.link">
      {{ info.name }}
    </a> - Some rights reserved. &nbsp; v. {{ info.version }}
  </p>
</template>

<script setup>
import { ref } from "vue";
const info = ref({
  version: "0.1.8",
  name: "Trip Kendall",
  link: "https://github.com/TripKendall/front-end",
  year: new Date().getFullYear(),
});
</script>