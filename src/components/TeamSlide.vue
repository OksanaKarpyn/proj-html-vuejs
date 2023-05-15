<script>
export default {
    name: 'TeamSlide',
    components: {
    },
    data() {
        return {
            current: [1],
            play: null,
            listTeam: [

                {
                    img: '../../public/images/testimonial-avata-02.jpg',
                    title: 'MINA HOLLAGE',
                    prof: '/Freelancer'

                },
                {
                    img: '../../public/images/testimonial-avata-04.jpg',
                    title: 'MADLEY PONDOR',
                    prof: '/PrivateTotor'
                },
                {
                    img: '../../public/images/testimonial-avata-01.jpg',
                    title: 'lUVIC DUBBLE',
                    prof: '/ IT Specialist'
                },
                {
                    img: '../../public/images/testimonial-avata-03.jpg',
                    title: 'MADLEY PONDOR',
                    prof: '/PrivateTotor'

                },
            ]
        }
    },
    mounted() {
        this.autoplay()
    },
    methods: {
        prev() {
            if (this.current == 0) {
                this.current = this.listTeam.length - 1
            } else {
                this.current--
            }
        },
        next() {
            if (this.current == this.listTeam.length - 1) {
                this.current = 0
            } else {
                this.current++
            }
        },
        changeCard(i) {
            this.current = i
        },
        autoplay() {
            this.play = setInterval(() => {
                this.next()
            }, 3000)
        }

    }
}
</script>
<template>
    <main class="d-flex general">
        <div class=" main d-flex flex-start">
            <i class="fa-solid fa-angle-left prev" @click="prev"></i>
            <div v-for="(item, index) in listTeam" :key="index" class="item mt-5 d-flex "
                :class="(current == index ? 'd-block' : ' d-none')" @click="changeCard(index)">
                <div class="card" style="width: 26rem;">
                    <div class="img-container">
                        <img :src="item.img" class="" alt="foto">
                    </div>
                    <div class="card-body">
                        <p class="card-text">Some quick example text to build on the card title and make up the bulk of the
                            card's content.</p>
                        <h5 class="card-title"><strong>{{ item.title }}</strong></h5>
                        <div class="card-text">{{ item.prof }}</div>
                    </div>
                </div>
            </div>
            <i class="fa-solid fa-angle-right next" @click="next"></i>
        </div>

    </main>
</template>
<style lang="scss" scoped>
.main {
    position: relative;
    //border: 1px solid red;
    //overflow-x: hidden;
    margin-bottom: 100px;
    padding-top: 50px;

    .item {

        .card {
            position: relative;
            text-align: center;
            background-color: #fff;
            border: 0;


            .img-container {
                height: 50px;

                //text-align: center;
                img {

                    top: -50px;
                    left: 50%;
                    transform: translate(-50%);
                    position: absolute;
                    width: 100px;
                    //display: block;
                    border-radius: 50%;
                }
            }

            .card-body {
                p {
                    color: #3F3A64;
                    font-weight: 500;
                    padding: 10px 20px;
                }

                h5 {
                    font-size: 1.3rem;
                }
            }
        }


    }

    .prev {
        z-index: 1;
        top: 40%;
        position: absolute;
        color: #B6B7D2;
        font-size: 2rem;

    }

    .next {
        z-index: 1;
        top: 40%;
        font-size: 2rem;
        position: absolute;
        right: 0;
        color: #B6B7D2;

    }


}
</style>