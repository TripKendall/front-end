<template>
  <section class="footerWrapper">
    <h3> Latest News: </h3>
    <ul role="list" class="mt-4 space-y-4">
      <li v-for="item in cat" :key="item.name">
        <a :href="item.href" class="footerItem">
          {{ item.name }}
        </a>
      </li>
    </ul>
  </section>
</template>

<script setup>
const cat = [
  { name: "Your Privacy", href: "https://wlog.app/posts/PersonalPrivacy.html" },
  { name: "What are Passkeys?", href: "https://wlog.app/posts/passkeys.html" },
  { name: "Secure Network", href: "https://wlog.app/posts/secure-your-network-with-linux-and-squid.html" },
  { name: "Microsoft Teams", href: "https://wlog.app/posts/why-people-hate-microsoft-teams.html" },
];
</script> 