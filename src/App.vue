<script >
import { store } from './store';
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';

export default {
  name: 'AppVue',
  components: {
    HeaderComp,
    MainComp,
  },
  data() {
    return {
      store,
      darkMode: false
    }
  },
  methods: {
    toggle() {
      this.darkMode = !this.darkMode
    }
  }

}

</script>

<template>
  <div class="wrapper">
    <button class="btn  btn-outline-ligth dark" @click="toggle"
      :class="this.darkMode == true ? 'orange' : 'lilla'">click</button>
    <div class="content" :class="{ 'dark-mode': darkMode }">
      <header>
        <HeaderComp></HeaderComp>
      </header>
      <main>
        <MainComp></MainComp>
      </main>
      <footer></footer>
    </div>
  </div>
</template>

<style lang="scss">
@use '../src/style/main.scss';

.wrapper {
  position: relative;

  .dark {
    z-index: 2;
    position: absolute;
    top: 20px;
    right: 10px;
  }

  .lilla {
    background-color: #B6B7D2;
    color: #fff
  }

  .orange {
    background-color: #FB9300;

  }

  .dark-mode {
    background-color: #1f1f1f;
    color: coral;

    li {
      color: coral;


    }

    select {
      color: coral;

      option {
        color: #000;
      }
    }
  }
}
</style>
