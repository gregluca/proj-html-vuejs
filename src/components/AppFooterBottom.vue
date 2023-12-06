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
        <div class="box-main">
        <div class="box-left">
            <p>&copy; Copyright 2012-2020/ Avada Theme by <a href="">ThemeFusion</a> / All Rights Reserved / Powered by <a href="">WordPress</a></p>
        </div>
        <div class="box-right">
            <i class="fa-brands fa-facebook-f"></i>
            <i class="fa-brands fa-twitter"></i>
            <i class="fa-brands fa-youtube"></i>
            <i class="fa-brands fa-instagram"></i>
        </div>
    </div>
    </div>
</div>
</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
.big-container {
    background-color: #1c1d1e;
}
.small-container {
    width: 70%;
    margin: 0 auto;
}
.box-main {
    color: white;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 5rem;


    .box-left {
        p {
            font-size: .8rem;
            color: $btn-grey;
        }
        a {
            text-decoration: none;
            color: $green-color;
        }
    }
    .box-right {
        i {
            margin-right: 1rem;
        }
    }
}
</style>