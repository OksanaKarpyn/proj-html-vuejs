<script>
import NavListHeader from './NavListHeader.vue';
export default {
    name: 'HeaderComp',
    components: {
        NavListHeader,
    },
    data() {
        return {
            navList: [
                {
                    name: 'Home',
                },
                {
                    name: 'Pages',
                },
                {
                    name: 'Courses',
                },
                {
                    name: 'Features',
                },
                {
                    name: 'Blog',
                },
                {
                    name: 'Shop',
                },

            ]
        }
    }
}
</script>
<template>
    <header>
        <!--logo- nav -->
        <div class="container header-nav">
            <div class="logo me-5 mb-2">
                <img src="/public/images/dark-logo.png" alt="foto_logo" style="width: 110px;">
            </div>
            <NavListHeader v-for="(item, index) in this.navList" :key="index" :propsList="item"></NavListHeader>

            <div class="d-flex mx-1">
                <i class="fa-solid fa-cart-shopping mx-1"></i>
                <i class="fa-regular fa-user ms-1"></i>
            </div>
            <div class="d-flex bg-white">
                <input type="text" class="form-control ms-2 border-0 p-1 rounted" placeholder="Search"
                    aria-label="Recipient's username" aria-describedby="button-addon2">
                <button class="btn border-0" type="button" id="button-addon2"><i class="fa-solid fa-magnifying-glass"
                        style="color:#24AF98;"></i></button>
            </div>
        </div>
        <!-- header- article-img -->
        <div class=" header-block">
            <div class="header-main container mt-5">
                <div class="article pe-5">
                    <h1>Complete Your Dreams in JavaS Programming</h1>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptas, ab pariatur aut, illum commodi
                        libero
                        cumque odit beatae repellat, fugiat alias omnis consectetur qui.
                    </p>
                    <div class="">

                        <button class="btn p-2 mt-3">
                            <i class="fa-solid fa-download"></i>
                            <span class="p-2">Downloand free
                                E-book</span></button>
                    </div>
                </div>
                <div class="img">
                    <img src="/images/home-5-hero-image.png" alt="foto_hero" width="100%">
                </div>
            </div>
        </div>
        <div class="onde">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
                <path fill="#b6b8d1" fill-opacity="0.6"
                    d="M0,128L26.7,160C53.3,192,107,256,160,272C213.3,288,267,256,320,213.3C373.3,171,427,117,480,117.3C533.3,117,587,171,640,208C693.3,245,747,267,800,277.3C853.3,288,907,288,960,261.3C1013.3,235,1067,181,1120,170.7C1173.3,160,1227,192,1280,176C1333.3,160,1387,96,1413,64L1440,32L1440,320L1413.3,320C1386.7,320,1333,320,1280,320C1226.7,320,1173,320,1120,320C1066.7,320,1013,320,960,320C906.7,320,853,320,800,320C746.7,320,693,320,640,320C586.7,320,533,320,480,320C426.7,320,373,320,320,320C266.7,320,213,320,160,320C106.7,320,53,320,27,320L0,320Z">
                </path>
            </svg>
        </div>


    </header>
</template>
<style lang="scss" scoped>
header {
    padding-top: 10px;
    position: relative;

    .header-nav {
        background-color: none;
        padding: 10px;
        display: flex;
        justify-content: space-between;
        align-items: center;

        button {
            padding: 8px;
            background-color: #fff;
        }

        input {
            // font-size: .7rem;
            max-width: 300px;

        }
    }

    //fine-naw
    .header-block {

        .header-main {
            display: flex;
            justify-content: space-between;
            align-items: center;

            .article {
                max-width: 500px;


                h1 {
                    color: #3F3A64;
                    font-size: 3rem;
                    padding-bottom: 15px;
                    font-weight: bold;
                }

                p {
                    color: #908ca3;
                    line-height: 25px;
                    //font-size: .8rem;
                }

                .btn {
                    background-color: #20AD96;
                    color: #fff;
                    //font-size: .7rem;
                }
            }
        }


    }

    .onde {
        z-index: -1;
        position: absolute;
        background-color: #E9E6E3;
        bottom: 0px;
        width: 100%;
        height: 100%;

        svg {
            position: absolute;
            bottom: 0;
        }
    }
}
</style>