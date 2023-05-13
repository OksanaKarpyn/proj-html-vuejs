<script>
import MainDream from './MainDream.vue';
import DreamInfo from './DreamInfo.vue';
export default {
    name: 'MainComp',
    components: {
        MainDream,
        DreamInfo
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
</template>
<style lang="scss" scoped></style>