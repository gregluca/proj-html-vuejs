<script>
import AppButton from './AppButton.vue';


export default {
    data() {
        return {
            buttonText:"MORE FROM BLOG"
        };
    },
    components: { AppButton }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="row">
            <h2>Latest News</h2>
            <div class="l-card">
                <div class="car-img">
                    <img src="../assets/img/blog-choosecar-700x441.jpg" alt="">
                </div>
                <p><strong>What Car to Start With?</strong></p>
                <p>February 7th, 2019 /</p>
                <span> 0 Comments</span>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing</p>
            </div>
            <div class="r-card">
                <div class="car-img">
                    <img src="../assets/img/blogpost-10and2-700x441.jpg" alt="">
                </div>
                <p><strong>Avada Driving School Expanding</strong></p>
                <p>February 7th, 2019 /</p>
                <span> 0 Comments</span>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing</p>
            </div>
            <AppButton :buttonText="buttonText"/>
        </div>
        <div class="blogspot">
            <img src="../assets/img/latestnews-bottom.png" alt="">
        </div>
    </div>
</div>

</template>
<style scoped lang="scss">
.big-container {
    width: 100%;
    background-image: url(../assets/img/latestnews-background.jpg);
    background-size: cover;
    background-repeat: no-repeat;
}
.small-container {
    width: 70%;
    margin: 0 auto;
}
.row {
    background: white;
    padding: 1rem;
    display: flex;
    justify-content: center;
    text-align: center;
    
    .car-img {
        padding: 1rem;
    }

    h2 {
        padding: 3rem;
        text-align: center;
    }
    .l-card {
        width: 50%;
    }
    .r-card {
        width: 50%;
    }
}
img {
    width: 100%;
    display: block;
}
.car-img:hover{
    opacity: .5;
    transform: scale(1.1);
}
</style>