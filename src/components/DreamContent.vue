<script>
export default {
    name: 'DreamContent',
    components: {

    },
    data() {
        return {
        }
    },
    mounted() {
    },
    methods: {
    }
}
</script>
<template>
    <main>
        <div class="container">
            <div class="img-container">
                <img src="../../public/images/about-us-03-image-01.png" alt="foto">
            </div>
            <div class="body">
                <p>DREAM WITH <span><strong>MAX</strong></span><span><strong>COACH</strong></span></p>
                <h2 class="pb-5">Construct A <span class="stunning">Stunning</span> Career Perspective</h2>
                <!--------- accordion-->
                <div class="accordion" id="accordionExample">
                    <div class="accordion-item">
                        <h2 class="accordion-header">
                            <button class="accordion-button" type="button" data-bs-toggle="collapse"
                                data-bs-target="#collapseOne" aria-expanded="true" aria-controls="collapseOne">
                                Multiple Platform Supported for Teaching & Studying
                            </button>
                        </h2>
                        <div id="collapseOne" class="accordion-collapse collapse show" data-bs-parent="#accordionExample">
                            <div class="accordion-body">
                                MaxCoach supports the act of teaching and leaming on multiple platforms like online or
                                offline via material downloads. We know things aren't supposed to be devoured in a short
                                time, you can always access our knowledge base from any device.
                            </div>
                        </div>
                    </div>
                    <div class="accordion-item">
                        <h2 class="accordion-header">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                data-bs-target="#collapseTwo" aria-expanded="false" aria-controls="collapseTwo">
                                Multiple Course Participation at the Same Time
                            </button>
                        </h2>
                        <div id="collapseTwo" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                            <div class="accordion-body">
                                MaxCoach supports the act of teaching and leaming on multiple platforms like online or
                                offline via material downloads. We know things aren't supposed to be devoured in a short
                                time, you can always access our knowledge base from any device.
                            </div>
                        </div>
                    </div>
                    <div class="accordion-item">
                        <h2 class="accordion-header">
                            <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse"
                                data-bs-target="#collapseThree" aria-expanded="false" aria-controls="collapseThree">
                                Track Study Progress & Deliver Prompt Feedbacke
                            </button>
                        </h2>
                        <div id="collapseThree" class="accordion-collapse collapse" data-bs-parent="#accordionExample">
                            <div class="accordion-body">
                                MaxCoach supports the act of teaching and leaming on multiple platforms like online or
                                offline via material downloads. We know things aren't supposed to be devoured in a short
                                time, you can always access our knowledge base from any device.
                            </div>
                        </div>
                    </div>
                </div>
                <!---------fine.accordion -->
            </div>
        </div>
    </main>
</template>
<style lang="scss" scoped>
.container {
    display: flex;
    justify-content: space-between;
    align-items: center;

    .img-container {}

    .body {
        max-width: 600px;

        p {}

        h2 {
            color: #3F3A64;
            font-weight: bold;
            font-size: 3rem;

            .stunning {
                color: #20AD96;
                font-weight: 100;

            }
        }

        //accordion
        .accordion-item {
            margin-bottom: 20px;
            border: 0px;
            //shadow: 2px 2px 2px#F0F0F0;

            .accordion-button {
                font-weight: 600;
                background-color: #20AD96;
                color: #fff;
            }

            .accordion-body {
                background-color: #fff;
                letter-spacing: 1px;
                word-spacing: 1.5px;
            }
        }


    }
}
</style>