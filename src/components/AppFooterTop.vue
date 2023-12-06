<script>
import AppButton from './AppButton.vue';


export default {
    data() {
        return {
            buttonText:"BOOK NOW"
        };
    },
    components: { AppButton }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="row">
            <div class="col-3">
                <img src="../assets/img/avada-drivers-logo-1x.png" alt="">
                <p>Avada Driving School is the right choice for experienced drivers looking for a refrescher course, or the brand new driver wanting to pass first time.</p>
            </div>
            <div class="col-3">
                <h5>CONTACT DETAILS</h5>
                <ul>
                    <li>
                        <i class="fa-solid fa-house-chimney"></i>
                        <p>12345 North Main street, New York, NY 555555</p>
                    </li>
                    <li>
                        <i class="fa-solid fa-phone-flip"></i>
                        <p>1.800.555.6789</p>
                    </li>
                    <li>
                        <i class="fa-regular fa-envelope"></i>
                        <p>info@your-domain.com</p>
                    </li>
                    <li>
                        <i class="fa-solid fa-link"></i>
                        <p>Theme-Fusion.com</p>
                    </li>
                </ul>
            </div>
            <div class="col-3">
                <h5>COURSES</h5>
                <ul>
                    <li>
                        <i class="fa-regular fa-circle-right"></i>
                        <p><strong>Pass Plus</strong></p>
                    </li>
                    <li>
                        <i class="fa-regular fa-circle-right"></i>
                        <p><strong>Intensive Course</strong></p>
                    </li>
                    <li>
                        <i class="fa-regular fa-circle-right"></i>
                        <p><strong>Automatic</strong></p>
                    </li>
                    <li>
                        <i class="fa-regular fa-circle-right"></i>
                        <p><strong>Instructor Training</strong></p>
                    </li>
                </ul>
            </div>
            <div class="col-3">
                <div class="box">
                    <img src="../assets/img/footer-ad-grid-200x178.png" alt="">
                    <AppButton :buttonText="buttonText"/>
                </div>
            </div>
        </div>
    </div>
</div>
</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
.big-container{
    width: 100%;
    background-image: url(../assets/img/footer-background-color.jpg);
    background-size: cover;
    background-size: contain;
}
.small-container {
    width: 70%;
    margin: 0 auto;
}
.row {
    img {
        width: 200px;
    }
    h5 {
        color: white;
        text-align:start
    }
    color: $btn-grey;
    padding: 5rem;

}
.col-3 {
    .box {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 2rem;
    }
    ul {
        padding: 0;
        list-style-type: none;
        li {
            display: flex;
            
            line-height: 2rem;
            i {
                line-height: 2rem;
                margin-right: 1.5rem;
            }
        }
    }
}
</style>