<script>
import AppButton from './AppButton.vue';
import AppInstructorsCard from './AppInstructorsCard.vue';


export default {
    data() {
        return {
            buttonText:"MORE ABOUT US"
        };
    },
    components: { AppButton, AppInstructorsCard }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="row">
            <div class="card-group">
                <div class="card">
                    <div class="card-body">
                        <p class="card-text">95%</p>
                    </div>
                    <span>PASS RATE</span>
                </div>
                <div class="card">
                    <div class="card-body">
                        <p class="card-text">100%</p>
                    </div>
                    <span>RAFERRAL RATE</span>
                </div>
                <div class="card">
                    <div class="card-body">
                        <p class="card-text">0%</p>
                    </div>
                    <span>ACCIDENT RATE</span>
                </div>
</div>
        </div>
        <div class="center">
            <div class="box-left">
                <h3>Your Instructors</h3>
                <span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi dolore necessitatibus, minima illum perferendis earum eos dignissimos, velit unde maxime incidunt! </span>
            </div>
            <div class="right-box">
                <AppButton :buttonText="buttonText"/>
            </div>
        </div>
        <AppInstructorsCard />
    </div>
</div>
</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
.big-container {
    width: 100%;
}
.small-container {
    width: 70%;
    margin: 0 auto;

    .row {

        .col {
            width: calc(100% / 3);
            display: flex;
            justify-content: center;
            align-items: center;
        }
    }
    .center {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .box-left {
            padding: 5rem;
            width: 70%;
            span {
                color: $btn-grey;
            }
        }
        .right-box {
            width: 30%;
            margin-left: 5rem;
        }
}
.card {
    position: relative;
    top: -30px;
    padding: 3rem;
    margin-right: 1rem;
    box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);

    span {
        font-size: 1rem;
        color: $btn-grey;
        text-align: center;
    }
}
.card-body {
    display: flex;
    justify-content: center;
    align-items: center;
}
.card-text {
    text-align: center;
    border: 10px solid $green-color;
    width: 200px;
    height: 200px;
    border-radius: 50%;
    vertical-align: middle;
    display: flex;
    justify-content: center;
    align-items: center;

}
p {
    text-align: center;
    font-size: 3rem;
    color: $btn-grey;
}
</style>