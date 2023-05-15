<script>
import MainDream from './MainDream.vue';
import DreamInfo from './DreamInfo.vue';
import MainCourses from './MainCourses.vue';
import MainLearn from './MainLearn.vue';
import MainEvents from './MainEvents.vue';
import MainTeam from './MainTeam.vue';
import Footer from './Footer.vue';
export default {
    name: 'MainComp',
    components: {
        MainDream,
        DreamInfo,
        MainCourses,
        MainLearn,
        MainEvents,
        MainTeam,
        Footer,
    },
    data() {
        return {
        }
    }
}
</script>
<template>
    <div>
        <MainDream></MainDream>
    </div>
    <div>
        <DreamInfo></DreamInfo>
    </div>
    <div>
        <MainCourses></MainCourses>
    </div>
    <div>
        <MainLearn></MainLearn>
    </div>
    <div>
        <MainEvents></MainEvents>
    </div>
    <div>
        <MainTeam></MainTeam>
    </div>
    <div>
        <Footer></Footer>
    </div>
</template>
<style lang="scss" scoped></style>