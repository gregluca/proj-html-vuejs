<script>
import AppButton from './AppButton.vue';
export default {
    components: {AppButton},
    data() {
        return {
            buttonText: "SUBSCRIBE"
        }
    }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="news">
            <h2>Sign up to our Newsletter</h2>
            <input class="form-control w-75" type="text" aria-label="default input example">
            <AppButton :buttonText="buttonText"/>
            <p>(We don't share your data with anybody, and only use it for its intended purpose)</p>
        </div>
    </div>
</div>
</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
.big-container {
    background-image: url(../assets/img/newsletter_background.jpg);
    background-size: cover;
    width: 100%;
}
.small-container {
    width: 70%;
    margin: 0 auto;

    .news {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        align-items: center;
        gap: 2rem;
        padding: 3rem;
        
        h2 {
            text-align: center;
            width: 100%;
            font-size: 1.4rem;
        }

        p {
            font-size: .8rem;
            color: $btn-grey;
        }
    }
}
</style>