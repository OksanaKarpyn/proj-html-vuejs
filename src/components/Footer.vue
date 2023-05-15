<script>
import FooterList from './FooterList.vue';
export default {
    name: 'Footer',
    components: {
        FooterList,
    },
    data() {
        return {

        }
    }
}
</script>
<template>
    <main class="container">

        <div class="content">
            <div class="address">
                <ul>
                    <li>
                        <h5><strong>Address</strong></h5>
                    </li>
                    <li>382 NE 191st St # 87394 Miami, </li>
                    <li>FL 33179-3899 +1(305) 547-9909</li>
                    <li>(9am - 5pm EST, Monday - Friday)</li>
                    <li><a href="#">support@maxcoach.com</a></li>
                    <li>
                        <i class="fa-brands fa-facebook"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                        <i class="fa-brands fa-linkedin"></i>
                    </li>
                </ul>

                <p></p>
            </div>
            <div class="list">
                <FooterList></FooterList>
            </div>
        </div>
        <div class="max-footer">
            <i class="fa-regular fa-copyright"></i>
            <span>2020 Maxcoach.All Rights Reserved</span>
        </div>
    </main>
</template>
<style lang="scss" scoped>
.container {
    margin-top: 80px;
    margin-bottom: 80px;

    .content {
        display: flex;
        justify-content: space-around;

        .address {
            ul {
                li {
                    padding-bottom: 10px;
                    color: #807d7d;

                    h5 {
                        color: #000;
                    }

                    a {
                        //text-decoration: none;
                        color: #807d7d;
                    }

                    i {
                        padding-top: 25px;
                        padding-right: 30px;
                        font-size: 1.6rem;
                    }
                }
            }

        }
    }

    .max-footer {
        margin-top: 10px;
        display: flex;
        justify-content: center;
        color: #807d7d;

    }
}
</style>