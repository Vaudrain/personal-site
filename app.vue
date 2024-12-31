<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtLayout>
      <NuxtPage class="page" :page-key="route => route.fullPath == '/' ? landing : route.fullPath" />
    </NuxtLayout>
  </div>
</template>

<script setup>
import '~/assets/css/main.scss';
useHead({
  title: 'Vaud',
  viewport: 'width=device-width, initial-scale=1',
  charset: 'utf-8',
  meta: [{ name: 'description', content: 'Vaud' }],
  link: [{ rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' }],
})
</script>

<style lang="scss" scoped>
.page {
}
</style>