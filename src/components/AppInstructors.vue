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
            <div class="col">
                <h2>95%</h2>
            </div>
            <div class="col">
                <p>ciao</p>
            </div>
            <div class="col">
                <p>ciao</p>
            </div>
        </div>
        <div class="center">
            <div class="box-left">
                <h3>Your Instructors</h3>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi dolore necessitatibus, minima illum perferendis earum eos dignissimos, velit unde maxime incidunt! </p>
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
            border: 1px solid black;
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
            width: 70%;
            p {
                color: $btn-grey;
            }
        }
        .right-box {
            width: 30%;
            margin-left: 5rem;
        }
}
</style>