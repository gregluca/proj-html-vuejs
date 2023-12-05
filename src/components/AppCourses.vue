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
        <div class="row">
            <div class="col">
                <div class="card-car">
                    <img src="../assets/img/courses-passplus-200x200.jpg" alt="">
                    <h4>Pass Plus</h4>
                    <button><a href=""></a>LEARN MORE</button>
                </div>
            </div>
            <div class="col">
                <div class="card-car">
                    <img src="../assets/img/course-intensive-200x200.jpg" alt="">
                    <h4>Intensive Course</h4>
                    <button><a href=""></a>LEARN MORE</button>
                </div>
            </div>
            <div class="col">
                <div class="card-car">
                    <img src="../assets/img/courses-instructor-200x200.jpg" alt="">
                    <h4>Instructors</h4>
                    <button><a href=""></a>LEARN MORE</button>
                </div>
            </div>
        </div>
    </div>
</div>
</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
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
    display: flex;
    align-items:flex-end;

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
        width: 40%;
        text-align: center;
        padding: 3rem;
        border: none;
        border-radius: 5px;
        position: relative;
        top: -30px;
        p {
            color: $btn-grey;
        }
    }
    .row {
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: nowrap;
        width:60%;
        margin-left: 10%;
        padding-bottom: 2rem;
        
        h4 {
            padding-top: 2rem;
            text-align: center;
            color: $btn-grey;
        }
        .card-car  {
                text-align: center;
                
            button {
                text-decoration: none;
                border: 2px solid $btn-grey;
                color: $btn-grey;
                border-radius: 1rem;
                padding: 5px;
                background: none;
                font-size: .8rem;
                width: 100px;
            }
            a {
                text-decoration: none;
            }
        }
    }
}
</style>