<script>

export default {
    data(){
        return {
            testimonials: [
                {
                    name:"Sophia Jones",
                    image:"src/assets/img/testimonial-sophia.png",
                },
                {
                    name:"Kelly",
                    image:"src/assets/img/testimonial-kelly.png",
                },
                {
                    name:"Kate",
                    image:"src/assets/img/testimonial-kate.png",
                },
                {
                    name:"Harold",
                    image:"src/assets/img/testimonial-harold.png",
                },
                {
                    name:"Grant",
                    image:"src/assets/img/testimonial-grant.png",
                }
            ],
            currentIndex: 0,
        };
    },
    methods: {
        changeSlide(index) {
            this.currentIndex = index;
        },
        prevSlide() {
            this.currentIndex = (this.currentIndex - 1 + this.images.length) % this.images.length;
        },
        nextSlide() {
            this.currentIndex = (this.currentIndex + 1) % this.images.length;
        },
    },
};
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="box-monials">
            <h3>Testimonials</h3>
            <p>Here's what our happy drivers had to say about our services</p>
            <img :src="testimonials[currentIndex].image" alt="">
            <p>Avada Driving School really helped build my confidence behind the wheel and with driving in general. and they got me a first time pass! Higly recommended.</p>
            <p><strong>{{ testimonials[currentIndex].name }}</strong></p>
            <i v-for="(testimonial, index) in testimonials" :key="index" @click="changeSlide(index)" class="fa-regular fa-circle" :class="{ 'fa-solid': index === currentIndex }"></i>
        </div>
    </div>
</div>

</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
.big-container {
    width: 100%;
    height: 600px;
    background-image: url(../assets/img/testimonial-background.jpg);
    background-size: contain;
    background-size: cover;
    background-repeat: no-repeat;
}
.small-container {
    width: 70%;
    margin: 0 auto;

    .box-monials {
        text-align: center;
        padding-top: 5rem;
        p {
            color: $btn-grey;
        }

        img {
            width: 150px;
            margin: 2rem;
        }

        i {
            color: $btn-grey;
            margin: 1rem;
            font-size: 1rem;
            cursor: pointer;
        }
    }
    img:active {
        transform: scale(2);
    }
}
</style>