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
                <div class="box-grey">
                <h5>CONTACT DETAILS</h5>
                <ul>
                    <li>
                        <i class="fa-solid fa-house-chimney"></i>
                        <p><a href="">12345 North Main street, New York, NY 555555</a></p>
                    </li>
                    <li>
                        <i class="fa-solid fa-phone-flip"></i>
                        <p><a href="">1.800.555.6789</a></p>
                    </li>
                    <li>
                        <i class="fa-regular fa-envelope"></i>
                        <p><a href="">info@your-domain.com</a></p>
                    </li>
                    <li>
                        <i class="fa-solid fa-link"></i>
                        <p><a href="">Theme-Fusion.com</a></p>
                    </li>
                </ul>
                </div>
            </div>
            <div class="col-3">
                <h5>COURSES</h5>
                <div class="box-green">
                <ul>
                    <li>
                        <i class="fa-regular fa-circle-right"></i>
                        <p><strong><a href="">Pass Plus</a></strong></p>
                    </li>
                    <li>
                        <i class="fa-regular fa-circle-right"></i>
                        <p><strong><a href="">Intensive Course</a></strong></p>
                    </li>
                    <li>
                        <i class="fa-regular fa-circle-right"></i>
                        <p><strong><a href="">Automatic</a></strong></p>
                    </li>
                    <li>
                        <i class="fa-regular fa-circle-right"></i>
                        <p><strong><a href="">Instructor Training</a></strong></p>
                    </li>
                </ul>
                </div>
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
        padding-bottom: 1rem;
        color: white;
        text-align:start
    }
    color: $btn-grey;
    padding: 5rem;

}
.col-3 {
    .box-grey {
        a {
            text-decoration: none;
            color: $btn-grey;
        }
        p:hover {
            opacity: .6;
        }
    }
    .box-green {
        color: $green-color;

        a {
            text-decoration: none;
            color: $green-color;
        }
        p:hover {
            opacity: .6;
        }
    }

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