<script>
export default {
    name: 'CoursesCard',
    props: ['propsListCourse'],
    components: {
    },
    data() {
        return {
        }
    }
}
</script>
<template>
    <!-- <img src="../../public/images/course-featured-image-01-480x298.jpg" alt=""> -->
    <div class="card border-0" style="width: 24rem;">
        <div class="img-container">
            <img :src="propsListCourse.img" class="card-img-top" alt="foto">
            <div class="label"><span>{{ propsListCourse.discount }}</span></div>
        </div>
        <div class="card-body text-start">
            <div class="img-card">
                <img :src="propsListCourse.ava" alt="foto" class="img-body">
                <p>{{ propsListCourse.name }}</p>
            </div>
            <h5 class="card-title py-2 mb-4"><strong>{{ propsListCourse.title }}</strong></h5>
            <div class="text-block d-flex">
                <p class="card-text">
                    <i class="fa-regular fa-file"></i>
                    <span class="me-1 ms-2">{{ propsListCourse.num1 }}</span>
                    <span>lessons</span>
                </p>
                <p class="card-text ms-4">
                    <i class="fa-regular fa-user"></i>
                    <span class="me-1 ms-2">{{ propsListCourse.num2 }}</span>
                    <span>Students</span>
                </p>
            </div>

        </div>
    </div>
</template>
<style lang="scss" scoped>
.card {
    background-color: transparent;

    .img-container {
        position: relative;

        // .label {
        // border-bottom-left-radius: 5px;
        // top: 0;
        // right: 0;
        // position: absolute;
        // font-weight: 800;
        // font-size: 1rem;
        // padding: 3px;
        // width: 80px;
        // height: 40px;
        // background-color: #20AD96;
        // text-align: center;
        // line-height: 30px;
        // color: #fff;

        //.span {
        // display: inline-block;
        // padding: 5px 8px;
        //}
        // }
    }

    .card-body {
        .img-card {
            p {
                display: inline-block;
                padding-left: 15px;
            }

            .img-body {
                border-radius: 50%;
            }
        }
    }
}
</style>