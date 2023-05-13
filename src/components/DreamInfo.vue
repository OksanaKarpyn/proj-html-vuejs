<script>

export default {
    name: 'DreamInfo',
    components: {
    },
    data() {
        return {
            listInfo: [
                {
                    num: '1.926',
                    text: 'FINISHED SESSIONS'
                },
                {
                    num: '3.092+',
                    text: 'ENROLLED LEARNERS'
                },
                {
                    num: '200',
                    text: 'ONLINE INSTRUCTORS'
                },
                {
                    num: '100%',
                    text: 'SATISFACTION RATE'
                },
            ]
        }
    },
    mounted() {

    },
    methods: {
        ramdom(max, min) {
            let random = Math.floor(Math.random() * max) + min;
            this.listInfo.push(random)
            return random
        }
    }

}
</script>
<template>
    <div class="block-info py-4 my-5">
        <div class=" container">
            <div v-for="(item, index) in listInfo" :key="index" class="num_info py-4">
                <h2>{{ item.num }}</h2>
                <p><strong>{{ item.text }}</strong></p>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.block-info {
    background-color: #FAF8F6;

    .container {
        display: flex;
        justify-content: space-around;

        .num_info {
            text-align: center;

            h2 {
                font-size: 3rem;
                font-weight: bold;
                color: #20AD96;
            }

            p {
                letter-spacing: 1.2px;
                color: #3F3A69;
            }
        }
    }

}
</style>