<script>
import TeamSlide from './TeamSlide.vue';
export default {
    name: 'MainTeam',
    components: {
        TeamSlide
    },
    data() {
        return {

        }
    }
}
</script>
<template>
    <main>

        <div class="container">
            <div class="main-header-team">
                <p>PEOPLE ARE PRAISING MAXCOACH</p>
                <h2>What make they <span>love us?</span></h2>
            </div>
            <div class="slide">
                <TeamSlide></TeamSlide>
            </div>
        </div>
        <div class="main-footer container">
            <img src="../../public/images/maxcoach-shape-01.png" alt="" class="line">
            <div>
                <h3>Start today for getting <span>Online Certification</span></h3>
                <h2>You can be your own guiding star with our help!</h2>
                <div class="">
                    <button class="btn p-3 px-5  mt-3">
                        <span class="py-3 px-2"><strong>Get started now</strong></span>
                    </button>
                </div>
            </div>
            <img src="../../public/images/maxcoach-shape-02.png" alt="" class="circle">
        </div>
    </main>
</template>
<style lang="scss" scoped>
main {
    background-color: #F8F8F8;

    .container {
        display: flex;
        justify-content: space-around;
        align-items: center;

        .main-header-team {
            max-width: 400px;

            p {
                letter-spacing: 1px;
                font-size: .9rem;
                text-align: center;
                font-weight: 600;
                color: #6d6c6c;
            }

            h2 {

                text-align: center;
                color: #3F3A64;
                font-weight: bold;
                font-size: 3rem;
                padding-bottom: 30px;

                span {
                    color: #20AD96;
                    font-weight: 100;
                    margin-left: 10px;
                }
            }
        }

    }

    .main-footer {
        text-align: center;
        position: relative;
        padding-bottom: 100px;
        //border: 1px solid red;

        .line {
            position: absolute;
            left: 150px;
        }

        .circle {
            position: absolute;
            right: 100px;
            bottom: 50px;
        }

        h3 {
            color: #3F3A64;

            span {
                color: #20AD96;
                font-weight: 100;
            }
        }

        h2 {
            padding-bottom: 20px;
            color: #3F3A64;
            font-weight: 700;
            font-size: 2rem;
        }

        .btn {
            margin: auto;
            background-color: #20AD96;
            color: #fff;
            //font-size: .7rem;
        }
    }
}
</style>