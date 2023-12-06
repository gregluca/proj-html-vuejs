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
            <a href=""><i class="fa-brands fa-facebook-f"></i></a>
            <a href=""><i class="fa-brands fa-twitter"></i></a>
            <a href=""><i class="fa-brands fa-youtube"></i></a>
            <a href=""><i class="fa-brands fa-instagram"></i></a>
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
        a:hover {
            opacity: .6;
        }
    }
    .box-right {
        a {
            text-decoration: none;
            color: $btn-grey;
        }
        i {
            margin-right: 1rem;
        }
        i:hover {
            opacity: .6;
        }
    }
}
</style>