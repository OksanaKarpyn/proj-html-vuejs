<script>
export default {
    name: 'FooterList',
    components: {
    },
    data() {
        return {
        }

    }
}
</script>
<template>
    <div class="list-items ">
        <div>
            <ul>
                <li>
                    <h5><strong>Explore</strong></h5>
                </li>
                <li>Start here</li>
                <li>Blog</li>
                <li>Abou us</li>
            </ul>
        </div>
        <div>
            <ul>
                <li class="invisible">
                    <h5><strong>invisible</strong> </h5>
                </li>
                <li>Success story</li>
                <li>Courses</li>
                <li>Contact us</li>
            </ul>
        </div>
        <div>
            <ul>
                <li>
                    <h5><strong>Information</strong></h5>
                </li>
                <li>Membership</li>
                <li>Purchase guide</li>
                <li>Privacy policy</li>
                <li>Terms of services</li>

            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.list-items {
    display: flex;

    ul {
        padding-right: 40px;
        margin-left: 10px;

        li {
            padding-bottom: 10px;
            color: #807d7d;

            h5 {
                color: #000;
            }
        }

        .invisible {
            visibility: 0;
        }
    }
}
</style>