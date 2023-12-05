<script>

export default {
    data() {
        return {

        }
    }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="news">
            <h2>Sign up to our Newsletter</h2>
            <input class="form-control w-25" type="text" >
        </div>
    </div>
</div>
</template>
<style scoped lang="scss">
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
        justify-content: center;
        
    }
}
</style>