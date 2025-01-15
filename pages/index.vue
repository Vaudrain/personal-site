<template>
    <div class="page">
        <div class="contents">
            <!-- <ComingSoon/> -->
            
        </div>   
    </div> 
</template>

<style lang="scss" scoped>
@use '~/assets/css/main.scss' as colours;
.page {
    height: 200vh;
    display: flex;
}

.contents {
    position: fixed;
    z-index: -2;
    background-color: wheat;
    height: 100%;
    width: 100%;
    overflow: hidden;
    display: flex;
    object-fit: contain;
    justify-content: center;
    align-items: center;
}

</style>