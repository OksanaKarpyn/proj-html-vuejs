<script>
import MainDream from './MainDream.vue';
import DreamInfo from './DreamInfo.vue';
import MainCourses from './MainCourses.vue';
import MainLearn from './MainLearn.vue';
import MainEvents from './MainEvents.vue';

export default {
    name: 'MainComp',
    components: {
        MainDream,
        DreamInfo,
        MainCourses,
        MainLearn,
        MainEvents,
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
</template>
<style lang="scss" scoped></style>