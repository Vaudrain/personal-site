<template>
    <div class="page">
        <BackgroundDots/>
        <div class="contents">
            <CV/>
            
        </div>   
    </div> 
</template>

<style lang="scss" scoped>
@use '~/assets/css/main.scss' as colours;
.page {
    display: flex;
}

.contents {
    margin: 10px;
    height: 100%;
    width: 100%;
    overflow: hidden;
    display: flex;
    object-fit: contain;
    justify-content: center;
}

</style>