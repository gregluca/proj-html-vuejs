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
    <div class="box-icon">
                <div class="card">
                    <i class="fa-solid fa-lemon"></i>
                    <p>Demos</p>
                </div>
            </div>
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
        width: 70%;
        margin: 0 auto;
        color: white;

        .center-text {
            position: absolute;
            top: 25%;
            letter-spacing: 5px;
        }
    }
}
.box-icon {
    position: relative;
    top: -10px;
    left: -20px;
    display: flex;
    justify-content: end;
}
.card {
    display: flex;
    align-items: center;
    text-align: center;
    width: 50px;
    height: 50px;
    font-size: .8rem;
}
</style>