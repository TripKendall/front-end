<template>
  <div class="mt-12 md:mt-0 footerWrapper">
    <h3 class="text-sm font-medium text-gray-400">External:</h3>
    <ul role="list" class="mt-4 space-y-4">
      <li v-for="item in external" :key="item.name">
        <a :href="item.href" class="footerItem">
          {{ item.name }}
        </a>
      </li>
    </ul>
  </div>
</template>

<script setup>
const external = [
  { name: "My Resume", href: "https://github.com/TripKendall/resume" },
  { name: "Me on Twitter", href: "https://twitter.com/trip_kendall" },
  { name: "Get This Code", href: "https://github.com/TripKendall/front-end" },
  { name: "wLog.app", href: "https://wlog.app" },
]
</script>