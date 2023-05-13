<script>
export default {
    name: 'MainLearn',
    components: {
    },
    data() {
        return {
        }
    }
}
</script>
<template>
    <main class="container">
        <div class="first-container">
            <div class="body">
                <div class="main-header">
                    <p>WHY HESITATE TO REGISTER?</p>
                    <h2>Learn At Your Own<span> Pace</span></h2>
                </div>
                <div class="list">
                    <ul>
                        <li><i class="fa-solid fa-check"></i><span>Select & customize courses to your preferences</span>
                        </li>
                        <li><i class="fa-solid fa-check"></i><span>Change the tutor and make arrangements</span></li>
                        <li><i class="fa-solid fa-check"></i><span>Participate in events to join others</span></li>
                        <li><i class="fa-solid fa-check"></i><span>Get the desired certificate delivered at house</span>
                        </li>
                    </ul>
                </div>
                <div class="ms-3">
                    <button class="btn p-3 px-5  mt-3">
                        <span class="py-3 px-2"><strong>Get started for free</strong></span>
                    </button>
                </div>
            </div>
            <div class="img-container d-dlex">
                <img src="../../public/images/home-5-image-01.png" alt="foto" width="100%">
                <img src="../../public/images/maxcoach-shape-05-150x150.png" alt="" class="circle">
            </div>
        </div>
        <div class="second-container">
            <div class="img-container">
                <img src="../../public/images/home-5-image-02.png" alt="">
                <img src="../../public/images/maxcoach-shape-01.png" alt="" class="linee">
                <div>
                    <img src="../../public/images/maxcoach-shape-02.png" alt="" class="circle">
                    <img src="../../public/images/maxcoach-shape-07-150x150.png" alt="" class="retangle">
                </div>
            </div>
            <div class="body">
                <p>WHAT ARE YOU LOOKING FOR?</p>
                <h2>Learn on your <span>mobile</span> anytime!</h2>
                <p>Save lessons for later and revise or write notes at any time and on
                    dra multiple devices on your way. Never interfere with activities of dritto enjoymenor other precious
                    moments.
                </p>
                <div class="">
                    <button class="btn p-3 px-5  mt-3">
                        <span class="py-3 px-2"><strong>Download Our App</strong></span>
                    </button>
                </div>
            </div>
        </div>

    </main>
</template>
<style lang="scss" scoped>
.first-container {
    margin-top: 200px;
    display: flex;
    justify-content: space-around;
    align-items: start;

    .body {
        max-width: 400px;

        .main-header {
            p {
                letter-spacing: 1px;
                padding-bottom: 20px;
            }

            h2 {
                padding-bottom: 20px;
                color: #3F3A64;
                font-weight: 700;
                font-size: 3rem;

                span {
                    color: #20AD96;
                    font-weight: 100;
                }
            }

        }

        .list {
            ul {
                li {
                    padding-bottom: 10px;

                    i {
                        color: #20AD96;
                        margin-right: 10px;
                    }

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

    .img-container {
        position: relative;
        display: flex;
        background-image: url(../../public/underlay-shape-grey.svg);
        background-size: 380px 650px;
        background-repeat: repeat-y;

        img {
            display: block;
        }

        .circle {
            position: absolute;
            align-self: center;
            right: -80px;
            bottom: 80px;

        }
    }
}

.second-container {
    margin-top: 50px;
    display: flex;
    justify-content: space-around;
    align-items: center;

    .img-container {
        width: 600px;
        background-image: url(../../public/underlay-shape-grey.svg);
        position: relative;
        background-size: 555px 780px;
        background-repeat: repeat-y;
        // background-size: contain;
        background-position: left;
        display: flex;

        img {
            display: block;
        }

        .linee {
            position: absolute;
            align-self: center;
            left: -80px;
            top: 150px;
        }

        div {
            position: relative;
            display: flex;
            flex-direction: column;

            .circle {
                position: absolute;
                top: 80px;
                left: 50px;
            }

            .retangle {
                position: absolute;
                left: 0px;
                bottom: 30px;
            }
        }
    }

    .body {
        max-width: 500px;

        p {
            padding-bottom: 20px;
        }

        h2 {
            padding-bottom: 20px;
            color: #3F3A64;
            font-weight: 700;
            font-size: 3rem;

            span {
                color: #20AD96;
                font-weight: 100;
            }
        }

        .btn {
            margin: auto;
            background-color: #20AD96;
            color: #fff;
        }
    }
}
</style>