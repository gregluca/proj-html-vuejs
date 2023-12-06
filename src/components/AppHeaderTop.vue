<script>

export default {
    data(){
        return {

        }
    }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="box">
            <div class="top-left">
            <p>We have a 95% Successful Pass Rate!</p>
        </div>
        <div class="top-right">
            <p>Give us a call to book your tuition! 1-800-555-555</p>
        </div>
        </div>
    </div>
</div>
</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
.big-container {
    width: 100%;
    background-color: #353637;
    opacity: .8;
    color: $btn-grey;
    height: 30px;
}
.small-container {
    width: 70%;
    margin: 0 auto;
}
.box {
    display: flex;
    justify-content: space-between;
    color: grey;
    font-size: .8rem;
    padding: 10px;
}
</style>