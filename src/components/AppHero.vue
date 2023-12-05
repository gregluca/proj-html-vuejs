<script>


export default {
    data() {
        return {
        };
    },
}
</script>

<template>
<div class="big-container">
    <div class="small-container">
        <div class="center-text">
            <h1>Drive with Avada</h1>
            <p>We offer the finest driving tuition money we can buy</p>
        </div>
    </div>
</div>
    
</template>

<style scoped lang="scss">
.big-container {
    width: 100%;
    height: 500px;
    background-image: url(../assets/img/homepage-hero-background.jpg);
    background-size: contain;
    background-size: cover;

    .small-container {
        width: 80%;
        margin: 0 auto;
        color: white;

        .center-text {
            position: fixed;
            top: 25%;
            letter-spacing: 5px;
        }
    }
    
}
</style>