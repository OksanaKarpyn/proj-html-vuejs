<script >
import { store } from './store';
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';

export default {
  name: 'AppVue',
  data() {
    return {
      store,
    }
  },
  components: {
    HeaderComp,
    MainComp,
  }
}

</script>

<template>
  <header>
    <HeaderComp></HeaderComp>
  </header>
  <main>
    <MainComp></MainComp>
  </main>
  <footer></footer>
</template>

<style lang="scss">
@use '../src/style/main.scss';
</style>
