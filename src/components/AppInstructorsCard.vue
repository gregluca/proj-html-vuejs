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
                    image: "instructor-johnsmith",
                    description: "Lorem ipsum, dolor sit amet consectetur adipisicing elit. Libero, porro consectetur."
                },
                {
                    name:"Angela Hart",
                    image: "instructor-angelahart",
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
        <div class="instructos-box">
        <div class="row">
            <div class="col" v-for="(instructor, index) in instructors" :key="index">
                <div class="card">
                    <div class="img-container">
                        <img :src="`src/assets/img/${instructor.image}.jpg`" alt="">
                    </div>
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
}
.instructos-box {
    margin-top: 20px;
}
.row {
    display: flex;
    flex-wrap: nowrap;

    .col {

        .card {
            border-top: 6px solid $green-color;
            text-align: center;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
            p {
                color: $btn-grey;
            }
            h4 {
                font-size: 1rem;
            }
            
            .img-container {
                display: flex;
                align-items: center;
                justify-content: center;
                padding: 1rem;

                img {
                    width: 200px;
                }
            }

            .logos {
                color: $btn-grey;

                i {
                    margin-right: 1rem;
                }
            }
        }
        .card:hover{
            position: relative;
            transform: scale(1.2);
        }
    }
}
</style>