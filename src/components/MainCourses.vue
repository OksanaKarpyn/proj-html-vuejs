<script>
import CoursesCard from './CoursesCard.vue';
import CoursesCardBis from './CoursesCardBis.vue';
export default {
    name: 'MainCourses',
    components: {
        CoursesCard,
        CoursesCardBis,
    },
    data() {
        return {
            showList: false,
            listCourse: [
                {
                    img: '../../public/images/course-02-480x298.jpg',
                    discount: '$40.00',
                    ava: '../../public/images/73ee246daf47502812ccefc84bf02898.jpeg',
                    name: 'Blanche Fields',
                    title: 'Learning to Write as a Professional Author',
                    num1: '20',
                    num2: '50',
                },
                {
                    img: '../../public/images/stock-full-hd-03-480x298.jpg',
                    discount: 'Free',
                    ava: '../../public/images/d0d504142acfde820eef2f11feea6253.jpeg',
                    name: 'Maggie Strickland',
                    title: 'Customer-centric Info-Tech Strategies',
                    num1: '24',
                    num2: '769',
                },
                {
                    img: '../../public/images/stock-full-hd-04-480x298.jpg',
                    discount: '$19',
                    ava: '../../public/images/d0d504142acfde820eef2f11feea6253.jpeg',
                    name: 'Maggie Strickland',
                    title: 'Open Programming Courses for Everyone: Python',
                    num1: '17',
                    num2: '62',
                },
                {
                    img: '../../public/images/stock-full-hd-06-480x298.jpg',
                    discount: '$26',
                    ava: '../../public/images/73ee246daf47502812ccefc84bf02898.jpeg',
                    name: 'Blanche Fields',
                    title: 'Academic Listening and Note-taking for Beginners',
                    num1: '14',
                    num2: '67',
                },
                {
                    img: '../../public/images/course-featured-image-01-480x298.jpg',
                    discount: '$39',
                    ava: '../../public/images/73ee246daf47502812ccefc84bf02898.jpeg',
                    name: 'Blanche Fields',
                    title: 'Master jQuery in a Short Period of Time',
                    num1: '6',
                    num2: '51',
                },
                {
                    img: '../../public/images/stock-full-hd-05-480x298.jpg',
                    discount: '$59',
                    ava: '../../public/images/73ee246daf47502812ccefc84bf02898.jpeg',
                    name: 'Blanche Fields',
                    title: 'Introduction to Javascript for Beginners',
                    num1: '14',
                    num2: '76',
                },
            ],
            listCourseBis: [
                {
                    img: '../../public/images/course-02-480x298.jpg',
                    ava: '../../public/images/73ee246daf47502812ccefc84bf02898.jpeg',
                    name: 'Blanche Fields',
                    title: 'Learning to Write as a Professional Author',
                    num1: '20',
                    num2: '50',
                },
                {
                    img: '../../public/images/stock-full-hd-03-480x298.jpg',
                    ava: '../../public/images/d0d504142acfde820eef2f11feea6253.jpeg',
                    name: 'Maggie Strickland',
                    title: 'Customer-centric Info-Tech Strategies',
                    num1: '24',
                    num2: '769',
                },
                {
                    img: '../../public/images/stock-full-hd-04-480x298.jpg',
                    ava: '../../public/images/d0d504142acfde820eef2f11feea6253.jpeg',
                    name: 'Maggie Strickland',
                    title: 'Open Programming Courses for Everyone: Python',
                    num1: '17',
                    num2: '62',
                },
                {
                    img: '../../public/images/stock-full-hd-06-480x298.jpg',
                    ava: '../../public/images/73ee246daf47502812ccefc84bf02898.jpeg',
                    name: 'Blanche Fields',
                    title: 'Academic Listening and Note-taking for Beginners',
                    num1: '14',
                    num2: '67',
                },
                {
                    img: '../../public/images/course-featured-image-01-480x298.jpg',
                    ava: '../../public/images/73ee246daf47502812ccefc84bf02898.jpeg',
                    name: 'Blanche Fields',
                    title: 'Master jQuery in a Short Period of Time',
                    num1: '6',
                    num2: '51',
                },
                {
                    img: '../../public/images/stock-full-hd-05-480x298.jpg',

                    ava: '../../public/images/73ee246daf47502812ccefc84bf02898.jpeg',
                    name: 'Blanche Fields',
                    title: 'Introduction to Javascript for Beginners',
                    num1: '14',
                    num2: '76',
                },
            ]
        }
    },
    methods: {
        toggleList() {
            this.showList = !this.showList
        }
    }
}
</script>
<template>
    <main>
        <div class="bg">

            <div class="main-header-courses container">
                <p>CHOOSE WHERE YOU'D LIKE TO BEGIN</p>
                <h2>Latest Featured<span>Courses</span></h2>
                <div class="d-flex flex-wrap gap-4 justify-content-center py-4">
                    <CoursesCard v-for="(item, index) in listCourse" :key="index" :propsListCourse="item"></CoursesCard>
                    <div class="d-flex flex-wrap gap-4 justify-content-center py-4" v-if="showList">
                        <CoursesCardBis v-for="(item, index) in listCourseBis" :key="index" :propsListCourse="item">
                        </CoursesCardBis>
                    </div>
                </div>
            </div>
            <div class="d-flex">
                <button class="btn p-3 px-5  mt-3" @click="toggleList">
                    <span class="py-3 px-2"><strong>View all courses</strong></span>
                    <i class="fa-solid fa-arrow-right"></i>
                </button>
            </div>
        </div>
        <div class="onda">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
                <path fill="#F1F1F1" fill-opacity="1"
                    d="M0,32L120,53.3C240,75,480,117,720,112C960,107,1200,53,1320,26.7L1440,0L1440,0L1320,0C1200,0,960,0,720,0C480,0,240,0,120,0L0,0Z">
                </path>
            </svg>
        </div>
    </main>
</template>
<style lang="scss" scoped>
main {
    position: relative;

    .bg {
        position: relative;
        background: rgb(255, 255, 255);
        background: -moz-linear-gradient(180deg, rgba(255, 255, 255, 1) 4%, rgba(245, 245, 245, 1) 41%, rgba(244, 244, 244, 1) 64%, rgba(243, 243, 243, 1) 76%, rgba(241, 241, 241, 1) 97%);
        background: -webkit-linear-gradient(180deg, rgba(255, 255, 255, 1) 4%, rgba(245, 245, 245, 1) 41%, rgba(244, 244, 244, 1) 64%, rgba(243, 243, 243, 1) 76%, rgba(241, 241, 241, 1) 97%);
        background: linear-gradient(180deg, rgba(255, 255, 255, 1) 4%, rgba(245, 245, 245, 1) 41%, rgba(244, 244, 244, 1) 64%, rgba(243, 243, 243, 1) 76%, rgba(241, 241, 241, 1) 97%);
        filter: progid:DXImageTransform.Microsoft.gradient(startColorstr="#ffffff", endColorstr="#f1f1f1", GradientType=1);

        .main-header-courses {
            text-align: center;

            p {
                letter-spacing: 1px;
                font-size: .9rem;
                text-align: center;
            }

            h2 {

                text-align: center;
                color: #3F3A64;
                font-weight: bold;
                font-size: 2.8rem;
                padding-bottom: 30px;

                span {
                    color: #20AD96;
                    font-weight: 100;
                    margin-left: 10px;
                }
            }
        }

        .btn {
            margin: auto;
            background-color: #20AD96;
            color: #fff;
            //font-size: .7rem;
        }

    }

    .onda {
        position: absolute;
        //border: 1px solid rgb(28, 26, 26);
        height: 150px;
        bottom: -150px;
        width: 100%;


    }

}
</style>