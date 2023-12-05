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
        <div class="left-box">
            <h3>Start Learning to Drive Today</h3>
            <p>Give us a call to schedule your first driving lesson</p>
        </div>
        <div class="right-box">
            <h3><i class="fa-solid fa-phone"></i> 1-800-555-555</h3>
        </div>
    </div>
</div>
</template>
<style scoped lang="scss">
.big-container {
    background-image: url(../assets/img/horizontal-cta-background.jpg);
    background-size: contain;
    background-size: cover;
    padding:  4rem 0rem;
}
.small-container {
    width: 80%;
    margin: 0 auto;
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .right-box{
        h3 {
           padding-right: 5rem;
           i {
            margin-right: 2rem;
            text-align: center;
            transform: rotate(270deg);
            ;
           }
        }
    }
}
</style>