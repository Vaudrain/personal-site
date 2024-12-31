<template>
    <div class="page">
        <div class="text">COMING SOON</div>
        <div class="bg-image"></div>
        <NuxtImg class="face" src="/face.jpg"></NuxtImg>
        <div class="background">
            <div class="halftone"></div>
            <div class="halftone two"></div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '~/assets/css/main.scss' as colours;
.page {
    color: white;
    height: 100vh;
    width: 100vw;
    overflow: hidden;
    display: flex;
    object-fit: contain;
    justify-content: center;
    align-items: center;
}

.text {
    position: absolute;
    z-index: 3;
    box-shadow: 0 0 0 0 rgba(0, 0, 0, 1);
    transform: scale(1);
    animation: pulse 10s linear infinite;
}

.bg-image {
    overflow: hidden;
    z-index: 1;
    position: absolute;
    border: 3px solid colours.$accent;
    border-radius: 100000px;
    width: 50vw;
    height: 50vw;
	mix-blend-mode: multiply;
}

.face {
    overflow: hidden;
    z-index: 1;
    position: absolute;
    width: 50vw;
    height: 50vw;
    border-radius: 100000px;
}

.background {
    width: 100%;
    height: 100%;
    overflow: hidden;
	margin: 0;
	min-height: 100vh;
	display: grid;
	grid-template-columns: repeat(auto-fit,300%);
	grid-template-rows: repeat(auto-fit,130%);
	gap: 1rem;
	align-items: center;
	justify-content: center;
    background: linear-gradient(0deg, colours.$accent, colours.$accent2);
}

.halftone {
	--mask: linear-gradient(rgb(255, 255, 255), rgba(255, 255, 255, 0.35));
	--stop1: 3%;
	--stop2: 90%;

    height: 100%;
    width: 100%;
	
	aspect-ratio: 1;
	position: relative;
	background: black;
	filter: contrast(50);
	mix-blend-mode: multiply;
    grid: 0;
    grid-row-start: 1;
  grid-row-end: 1;
  grid-column-start: 1;
  grid-column-end: 1;
}

.halftone::after {
	content: '';
	position: absolute;
	inset: 0;
	mask-image: var(--mask);

	--bgSize: 60px;
	--bgPosition: calc(var(--bgSize) / 2);
	--stop1: 3%;
	--stop2: 60%;
	
	background-image: radial-gradient(circle at center, white var(--stop1), transparent var(--stop2)), radial-gradient(circle at center, white var(--stop1), transparent var(--stop2));
	background-size: var(--bgSize) var(--bgSize);
	background-position: 0 0, var(--bgPosition) var(--bgPosition);
    animation: move-right 10s ease-in-out infinite;
}

.two {
    animation: wobble 2.3s ease-in-out infinite;
    grid: 0;
}

@keyframes rotate {
    100% {
        transform:rotate(360deg); 
    }
}

@keyframes wobble {
    20% {
        transform: translate(2px,-1px);
    }

    54% {
        transform:translate(1px,2px); 
    }

    84% {
        transform: translate(-1px,-1px);
    }

    100% {
        transform:translate(0,0); 
    }
}

@keyframes move-right {
    25% {
        transform: translate(40px,-15px);
    }

    50% {
        transform:translate(80px,0); 
    }

    75% {
        transform: translate(40px,-15px);
    }

    100% {
        transform:translate(0,0); 
    }
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