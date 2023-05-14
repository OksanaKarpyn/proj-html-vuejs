<script>
export default {
    name: 'EventsCard',
    props: ['propseventsList'],
    components: {
    },
    data() {
        return {
        }
    }
}
</script>
<template>
    <div class="single-card col-5">
        <div class=" left">
            <p>
                <i class="fa-solid fa-location-dot pe-2"></i>
                <span>{{ propseventsList.country }}</span>
            </p>
            <h3><strong>{{ propseventsList.title }}</strong></h3>
        </div>
        <div class="right">
            <h2>{{ propseventsList.num }}</h2>
            <p><strong>{{ propseventsList.mount }}</strong></p>
            <button class="btn p-2 px-5 ">
                <span class="py-3 px-2"><strong>Get ticket</strong></span>
            </button>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.single-card {
    //max-width: 400px;
    background-color: #F8F8F8;
    padding: 20px;
    display: flex;
    justify-content: space-between;

    .left {
        min-height: 40px;

        p {
            color: #8C8C8C;
        }

        h3 {
            font-size: 1rem;
        }
    }

    .right {
        text-align: center;
        min-height: 40px;

        h2 {
            color: #20AD96;
            font-size: 2.5rem;
            margin-bottom: 0px;
        }

        p {
            margin-bottom: 0;
        }

        .btn {
            margin: auto;
            background-color: #20AD96;
            color: #fff;
            font-size: .8rem;
        }
    }
}
</style>