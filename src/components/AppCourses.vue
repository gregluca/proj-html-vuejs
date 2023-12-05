<script>
import AppButton from './AppButton.vue';


export default {
    data() {
        return {
            buttontext:"COURSE INFORMATION"
        };
    },
    components: { AppButton }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="card">
            <img src="../assets/img/new-corner.jpg" alt="">
            <h3>Courses</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Sapiente minima cumque provident esse voluptatem error, at quibusdam illum recusandae rem placeat nostrum, perferendis laborum quisquam delectus laudantium. Aspernatur, eligendi pariatur.</p>
            <AppButton :buttonText="buttontext"/>
        </div>
    </div>
</div>
</template>
<style scoped lang="scss">
.big-container {
    background-image: url(../assets/img/promise-background.jpg);
    background-size: contain;
    background-size: cover;
    background-repeat: no-repeat;
    width: 100%;
}
.small-container {
    width: 80%;
    margin: 0 auto;

    .card {
        img {
            position: absolute;
            width: 100px;
            top: 0;
            left: 0;
            border-radius: 5px;
        }
        h3 {
            padding: 1rem;
        }

        text-align: center;
        padding: 3rem;
        width: 30%;
        border: none;
        border-radius: 5px;
        position: relative;
        top: -30px;
    }
}
</style>