<template>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtLayout>
      <NuxtPage class="page" :page-key="route => route.fullPath == '/' ? landing : route.fullPath" />
    </NuxtLayout>
  </div>
</template>

<script setup lang="ts">
import '~/assets/css/main.scss';
useHead({
  title: 'Vaud',
  charset: 'utf-8',
  meta: [{ name: 'url', content:'vaud.uk' }, { name: 'description', content:'Nicholas Bentley' }, { name: 'type', content:'website' }, { name:'image', content:'/face.jpg'}],
  link: [{ rel: 'icon', type: 'image/x-icon', href: '/favicon.ico' }],
})
</script>

<style lang="scss" scoped>
.page {
}
</style>