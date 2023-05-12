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
        <div class="container border border-warning header">
            <div class="logo me-4 mb-2">
                <img src="../../public/images/dark-logo.png" alt="foto_logo" style="width: 110px;">
            </div>
            <NavListHeader v-for="(item, index) in this.navList" :key="index" :propsList="item"></NavListHeader>

            <div class="d-flex mx-1">
                <i class="fa-solid fa-cart-shopping mx-1"></i>
                <i class="fa-solid fa-user mx-1"></i>
            </div>
            <div class="input-group">
                <input type="text" class="form-control ms-2 border-0 border-bottom p-1 " placeholder="Search"
                    aria-label="Recipient's username" aria-describedby="button-addon2">
                <button class="btn  border-0 border-bottom" type="button" id="button-addon2"><i
                        class="fa-solid fa-magnifying-glass" style="color: #FB9300;"></i></button>
            </div>
        </div>
        <!-- header- article-img -->
        <div>
            <article>
                <h1>Complete Your Dreams in JavaS Programming</h1>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Voluptas, ab pariatur aut, illum commodi libero
                    cumque odit beatae repellat, fugiat alias omnis consectetur qui.
                </p>
            </article>
            <div class="img">
                <img src="" alt="">
            </div>
        </div>
    </header>
</template>
<style lang="scss" scoped>
.header {
    padding: 10px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    i {
        font-size: .8rem;
    }

    button {
        padding: 5px;
    }

    input {
        font-size: .7rem;
    }

    //fine nav

}
</style>