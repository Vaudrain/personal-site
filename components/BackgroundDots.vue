<template>
    <div class="background">
        <div class="halftone"></div>
        <div class="halftone two"></div>
    </div>
</template>

<style lang="scss" scoped>
@use '~/assets/css/main.scss' as colours;

.background {
    width: 100%;
    overflow: hidden;
	margin: 0;
	display: grid;
	grid-template-columns: repeat(auto-fit,300%);
	grid-template-rows: repeat(auto-fit,120%);
	gap: 1rem;
	align-items: center;
	justify-content: center;
    background: linear-gradient(0deg, colours.$accent, colours.$accent2);
    position: inherit;
    height: 100%;
}

.halftone {
	--mask: linear-gradient(rgb(255, 255, 255), rgba(255, 255, 255, 0.35));
	--stop1: 3%;
	--stop2: 90%;

    height: 200%;
    width: 100%;
	
	aspect-ratio: 1;
	position: relative;
	background: black;
	filter: contrast(20);
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
	
	background-image: radial-gradient(circle at center,
                                        white var(--stop1),
                                        transparent var(--stop2)),
                        radial-gradient(circle at center,
                                        white var(--stop1),
                                        transparent var(--stop2));
	background-size: var(--bgSize) var(--bgSize);
	background-position: 0 0, var(--bgPosition) var(--bgPosition);
    animation: orbit 30s linear infinite;
}

.two {
    animation: wobble 4s step-start infinite;
    grid: 0;
}

@keyframes rotate {
    100% {
        transform:rotate(360deg); 
    }
}


@keyframes orbit {
    from {  transform: rotate(0deg) translateX(40px) rotate(0deg); }
    to   {  transform: rotate(360deg) translateX(40px) rotate(-360deg); }
}

@keyframes wobble {
    0% {
        transform:translate(0,-2px); 
    }

    25% {
        transform: translate(2px,-1px);
    }

    50% {
        transform:translate(0px,2px); 
    }

    75% {
        transform: translate(-2px,-2px);
    }

    100% {
        transform:translate(0,-2px); 
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
        transform: translate(40px,15px);
    }
}
</style>