<template>
    <div class="text">COMING SOON</div>
    <NuxtImg class="face" src="/face.jpg"></NuxtImg>
</template>

<style lang="scss" scoped>
@use '~/assets/css/main.scss' as colours;

.text {
    position: absolute;
    z-index: 3;
    box-shadow: 0 0 0 0 rgba(0, 0, 0, 1);
    transform: scale(1);
    animation: pulse 10s linear infinite;
}

.face {
    overflow: hidden;
    z-index: 1;
    position: absolute;
    min-width: 200px;
    max-width: 30vw;
    min-height: 200px;
    max-height: 30vw;
    border-radius: 100000px;
    border: 3px solid colours.$accent;
}

@keyframes pulse {
    0% {
        transform: scale(1.1);
        filter: drop-shadow(0 0 0.1rem colours.$accent);
    }

    50% {
        transform: scale(1);
        filter: drop-shadow(0 0 0.2rem colours.$accent);
    }

    100% {
        transform: scale(1.1);
        filter: drop-shadow(0 0 0.1rem colours.$accent);
    }
}
</style>