<script lang="ts" setup>
import { navbarData } from '~/data'

useHead({
  title: 'Home',
  meta: [
    {
      name: 'description',
      content:
        'Welcome',
    },
  ],
  link: [
    {
      rel: 'icon',
      type: 'image/png',
      href: '/favicon.png'
    }
  ],
})

// Generate OG Image
defineOgImageComponent('About', {
  headline: 'Greetings',
  title: navbarData.homeTitle,
  description: 'Welcome to GOSIM',
  link: '/gosim-logo2.svg',
})
</script>

<template>
  <main class="container max-w-7xl mx-auto text-zinc-600">
    <MainHero />
    <MainRecent />
    <!-- <MainTrending /> -->
  </main>
</template>
