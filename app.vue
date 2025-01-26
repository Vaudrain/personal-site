<template>
  <Head>
    <html lang="en"></html>
    <meta property="og:locale" content="en_GB" />

    <title>Nic Bentley</title>

    <meta name="description" content="Nicholas Bentley - Developer & Researcher" />
    <meta name="author" content="Nicholas Bentley, nic@nicbentley.uk">
    <meta name="keywords" content="HTML, CSS, JavaScript, Full-stack, HCI, UX, Researcher, C#, Docker">
    <meta name='revised' content='Friday, January 24th, 2025'>
    <meta name='Classification' content='Portfolio'>
    <meta name='robots' content='index,follow'>

    <meta name='url' content='https://nicbentley.uk'>
    <link rel="canonical" href="https://nicbentley.uk" />
    <meta property="og:url" content="https://nicbentley.uk" />
    <meta property="twitter:domain" content="nicbentley.uk">
    <meta property="twitter:url" content="https://nicbentley.uk" />

    <meta property="og:title" content="Nic Bentley" />
    <meta name="twitter:title" content="Nic Bentley" />

    <meta property="og:description" content="Nicholas Bentley - Developer & Researcher" />
    <meta name="twitter:description" content="Nicholas Bentley - Developer & Researcher" />
    
    <meta property="og:image" content="https://nicbentley.uk/face.png"  />
    <meta property="twitter:image" content="https://nicbentley.uk/face.png"  />

    <meta name="twitter:card" content="summary_large_image" />
    <meta property="og:type" content="website" />

    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="icon" type="image/x-icon" href="/favicon.ico">
  </Head>
  <div>
    <NuxtRouteAnnouncer />
    <NuxtLayout>
      <NuxtPage/>
    </NuxtLayout>
  </div>
</template>

<script setup lang="ts">
import '~/assets/css/main.scss';
</script>