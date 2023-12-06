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
                <div class="box-center">
                    <p>February 7th, 2019 /</p>
                    <span> 0 Comments</span>
                </div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing</p>
            </div>
            <div class="r-card">
                <div class="car-img">
                    <img src="../assets/img/blogpost-10and2-700x441.jpg" alt="">
                </div>
                <p><strong>Avada Driving School Expanding</strong></p>
                <div class="box-center">
                    <p>February 7th, 2019 /</p>
                    <span> 0 Comments</span>
                </div>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing</p>
            </div>
            <div class="box-btn">
                <AppButton :buttonText="buttonText"/>
            </div>
        </div>
        <div class="blogspot">
            <img src="../assets/img/latestnews-bottom.png" alt="">
        </div>
    </div>
</div>

</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
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
    position: relative;
    top: -50px;
    border-top: 5px solid #7799ad ;
    border-radius: 10px 10px 5px 5px;
    background: white;
    padding: 1rem;
    display: flex;
    justify-content: center;
    text-align: center;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
    

     p {
        color: $btn-grey;
        font-size: .8rem;
     }
    .box-center {
        display: flex;
        justify-content: center;
        font-size: .8rem;
        p {
            color: $btn-grey;
        }
        span {
            color: $green-color;
        }
    }

    strong {
        font-size: 1.5rem;
        color: $green-color;
    }
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
    position: relative;
    top: -50px;
    width: 100%;
    display: block;
}
.car-img:hover{
    opacity: .5;
    transform: scale(1.1);
}
.blogspot {
   padding-bottom: 2rem;
}
.box-btn {
    margin: 3rem;
}
</style>