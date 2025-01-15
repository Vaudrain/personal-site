<template>
    <div class="banner">
        <BackgroundDots/>
    </div>
    <NuxtImg class="face" src="/face.jpg"></NuxtImg>
</template>

<style lang="scss" scoped>
@use '~/assets/css/main.scss' as colours;

.header {
    display: block;
}

.banner {
    height: 15vh;
    width: 100vw;
    top: 0;
    display: flex;
    background-color: aqua;
    border-bottom: 3px solid colours.$accent;
    position: absolute;
}

.face-container {
    position: sticky;
    top: 0px;
    background-color: transparent;
}

.face {
    z-index: 1;
    position: sticky;
    top: 10px;
    background-color: aqua;
    display: flex;
    justify-content: center;
    height: 8vh;
    margin: 10px;
    margin-top: 10vh;
    border-radius: 10px;
    border: 3px solid colours.$accent;
}

</style>