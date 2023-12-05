<script>

export default {
    data() {
        return {
            instructors: [
                {
                    name:"Mike Hart",
                    image: "instructor-mikehart",
                    description: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Libero, porro consectetur."
                },
                {
                    name:"John Smith",
                    image: "instructor-mikehart",
                    description: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Libero, porro consectetur."
                },
                {
                    name:"Angela Hart",
                    image: "instructor-mikehart",
                    description: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Libero, porro consectetur."
                }
            ]
        }
    }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="row">
            <div class="col" v-for="(instructor, index) in instructors" :key="index">
                <div class="card">
                    <img :src="`../assets/img/${instructor.image}.jpg`" alt="">
                    <h4>{{ instructor.name }}</h4>
                    <div class="logos">
                        <i class="fa-brands fa-facebook-f"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                    <p>{{ instructor.description }}</p>
                </div>
        </div>
    </div>
</div>
</div>
</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
.big-container {
    width: 100%;
}
.small-container {
    width: 80%;
    margin: 0 auto;
}
.row {
    width: 100%;

    .col {
        height: 100px;

        .card {
            img {
                width: 100px;
            }
        }
    }
}
</style>