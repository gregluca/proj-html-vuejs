<script>

export default {
    props: {
        elems: Array
    }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <img src="../assets/img/avada-drivers-logo-2x.png" alt="">
        <ul>
            <li v-for="(elem , index) in elems" :key="index"><a href="">{{ elem }}</a></li>
        </ul>
    </div>
</div>
</template>
<style scoped lang="scss">
.big-container {
    background-color: rgba(0,0,0,0.9);
    color: white;
}
.small-container {
    font-size: .8rem;
    width: 80%;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    padding: 1rem;

    img {
        height: 50px;
    }
    img:hover {
        opacity: .8;
    }

   ul {
    display: flex;
    justify-content: space-between;

    li {
        text-decoration: none;
        list-style-type: none;
        margin: 10px;
        letter-spacing: 3px;

        a {
            text-decoration: none;
            color: white;
        }
    }
    a:hover {
        color: green;
        border-bottom: 3px solid green;
        padding-top: 30px;
    }
   }
}
</style>