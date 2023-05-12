<script>
import DreamList from './DreamList.vue';
export default {
    name: 'MainDream',
    components: {
        DreamList
    },
    data() {
        return {
            listDream: [
                {

                    img: '/public/images/home-5-image-box-01.png',
                    name: 'IdeaDiscussion',
                    text: 'Get teamed up with the specialists who work and teach coding for years at famous universities.'
                },
                {
                    img: '/public/images/home-5-image-box-02.png',
                    name: 'Web Development',
                    text: 'Leam to start building a webpage from scratch. You decide your own pace, course and speed.',
                },
                {
                    img: '/public/images/home-5-image-box-03.png',
                    name: 'System Administration',
                    text: 'Leamers are encouraged to study the mechanism and structure of system administration.',
                },
                {
                    img: '/public/images/home-5-image-box-04.png',
                    name: 'Graphic Design',
                    text: 'Have a passion for graphics and arts? Show your talents with confidence and self-assertiveness.',
                },
            ]
        }

    }
}
</script>
<template>
    <main>
        <div class="container mt-5">
            <div class="main-header-dream mt-3 gap-2">
                <p>START LEARNING CODING LANGUAGES</p>
                <h2>Build Your Dream<span>TODAY</span></h2>
            </div>
            <div class=" cards d-flex my-5">
                <DreamList v-for="(item, index) in listDream" :key="index" :propsListDream="item"></DreamList>
            </div>
        </div>
    </main>
</template>
<style lang="scss" scoped>
.main-header-dream {
    p {
        letter-spacing: 1px;
        font-size: .7rem;
        text-align: center;
    }

    h2 {
        text-align: center;
        color: #3F3A64;
        font-weight: bold;

        span {
            color: #20AD96;
            font-weight: 100;
            margin-left: 10px;
        }
    }
}

.cards {}
</style>