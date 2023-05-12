<script>
export default {
    name: 'NavListHeader',
    props: ['propsList'],
    data() {
        return {

        }
    }
}
</script>
<template>
    <div>
        <ul>
            <li>
                <select class="form-select-xs border-0" aria-label="">
                    <option selected>{{ propsList.name }}</option>
                    <option value="1">One</option>
                    <option value="2">Two</option>
                    <option value="3">Three</option>
                </select>

            </li>
        </ul>
    </div>
</template>
<style lang="scss" scoped>
div {
    ul {
        margin-bottom: 0px;

        li {
            font-size: .6rem;

            select {
                background-color: transparent;

                option {
                    background-color: #523B5D;

                    &:hover {
                        background-color: #FB9000;

                    }
                }
            }
        }
    }
}
</style>