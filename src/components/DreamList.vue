<script>
export default {
    name: 'MainDream',
    props: ['propsListDream'],
    components: {

    },
    data() {
        return {
        }
    }
}
</script>
<template>
    <div class="card p-2">
        <div class=" img-container">
            <img :src="propsListDream.img" alt="...">
        </div>
        <div class="card-body">
            <h5 class="card-title"><strong>{{ propsListDream.name }}</strong></h5>
            <p class="card-text">{{ propsListDream.text }}</p>
            <a href="#" class="btn d-flex justify-content-center align-items-center"><span class="d-inline-block">Start
                    now</span><i class="fa-solid fa-arrow-right px-2 d-inline-block mt-1"></i></a>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.card {
    border: 0;

    .img-container {
        height: 200px;
        text-align: center;


        img {
            height: 100%;
        }
    }

    .card-body {
        text-align: center;

        h5 {}

        p {}
    }
}
</style>