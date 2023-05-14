<script>
import EventsCard from './EventsCard.vue';
export default {
    name: 'MainEvents',
    components: {
        EventsCard,
    },
    data() {
        return {
            eventsList: [
                {
                    country: 'Texas, US',
                    title: 'Storytelling Workshop',
                    num: '22',
                    mount: 'NOV',
                },
                {
                    country: 'New York, US',
                    title: 'Painting Art Contest 2020',
                    num: '10',
                    mount: 'DA',
                },
                {
                    country: 'Hamburg, Germany',
                    title: 'International Art Fair 2020',
                    num: '23',
                    mount: 'NOW',
                },
                {
                    country: 'Illinois, US',
                    title: 'Street Performance: Call for Artist',
                    num: '15',
                    mount: 'DEC',
                },
                {
                    country: 'Ilinois, US',
                    title: 'Consumer Food Safety Education',
                    num: '22',
                    mount: 'JUL',
                },
                {
                    country: 'Dubai',
                    title: 'How meditation improve your mental',
                    num: '12',
                    mount: 'AUG',
                }
            ]
        }
    }
}
</script>
<template>
    <main class="container my-5">
        <div class="main-header-events">
            <p>GET IN CONTACT NOW</p>
            <h2>Upcoming <span>Events</span></h2>
        </div>
        <div class="d-flex flex-wrap gap-5  justify-content-center">
            <EventsCard v-for="(item, index) in eventsList" :key="index" :propseventsList="item"></EventsCard>
        </div>
        <div class="link">
            <span>Excited about our event?</span>
            <a href="#">View all events <i class="fa-solid fa-arrow-right"></i></a>
        </div>
    </main>
</template>
<style lang="scss" scoped>
.main-header-events {
    text-align: center;
    margin-top: 150px;

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
        font-size: 2.8rem;
        padding-bottom: 30px;

        span {
            color: #20AD96;
            font-weight: 100;
            margin-left: 10px;
        }
    }
}

.link {
    letter-spacing: 1px;
    margin-top: 40px;
    display: flex;
    justify-content: center;

    span {
        font-weight: 600;
        color: #8C89A2;
    }

    a {
        margin-left: 5px;
        text-decoration: none;
        color: #20AD96;
        font-weight: 800;
    }

}
</style>