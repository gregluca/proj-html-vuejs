<script>
import AppButton from './AppButton.vue';


export default {
    data() {
        return {
            buttonText: "REQUEST A CALLBACK"
        };
    },
    components: { AppButton }
}
</script>
<template>
<div class="big-container">
    <div class="small-container">
        <div class="left-box ">
            <h3>Get behind The Wheel</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio omnis iusto nobis vero eos excepturi vel eligendi consequatur harum, debitis libero eaque quisquam, asperiores commodi ea sint, ducimus nemo eum!</p>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. A distinctio impedit, reprehenderit iusto dolores optio nostrum eveniet labore quod, aut numquam similique odio fuga magnam at nam. Quam, aperiam totam.</p>
        </div>
        <div class="right-box">
            <div class="card">
                <div class="title-card">
                    <h3>First Lesson Free!</h3>
                    <p>When u make a block booking with us your first lesson is included free.</p>
                </div>
                <div class="form p-3">
                    <input class="form-control" type="text" placeholder="Your Name" >
                    <input class="form-control" type="text" placeholder="Email">
                    <input class="form-control" type="text" placeholder="Telephone">
                    <input class="form-control" type="text" placeholder="Location">
                    <AppButton :buttonText="buttonText" />
                </div>
            </div>       
        </div>
    </div>
</div>
</template>
<style scoped lang="scss">
@use "../style/partials/variables" as *;
.big-container {
    padding: 1rem;
}
.small-container {
    width: 80%;
    margin: 0 auto;
    display: flex;

    .left-box{
        width: 60%;
        margin-right: 4rem;
        padding-top: 2rem;
        p {
            font-size: .9rem;
            padding-top: 1rem;
            line-height: 2rem;
            color: $btn-grey;
            letter-spacing: 2px;
        }
    }
    .right-box {
        position: relative;
        top: -50px;
        width: 40%;

    .card {
        padding-bottom: 2rem;
        border: none;
        box-shadow: 1px  1px 0px #dedede,
                    -1px -2px  #dedede,
                    -5px  10px 5px #dedede;
    }
    .form {     
        text-align: center;
        input {
            color: $btn-grey;
            background-color: #f7f7f7 ;
            margin-bottom: 1.5rem;
        }
    }
    .title-card {
        padding: 1rem 2rem;
            h3 {
                color: $green-color;
                padding-bottom: 1rem;
            }
            p {
                color: $btn-grey;
            }
            text-align: center;
        }
    }
}
</style>