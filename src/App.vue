<template>
  <div id="app">
    <Navbar/>
    <MainIcon></MainIcon>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import MainIcon from './components/MainIcon.vue';
import Navbar from './components/Navbar.vue';
import Wave from'./components/Wave.vue';

export default defineComponent({
  name: 'App',
  components: {
    MainIcon,
    Navbar,
    Wave
  }
});
</script>

<style>
/* Elimina márgenes del cuerpo y del navbar */
body {
  margin: 0;
  padding: 0;
}

#app {
  margin: 0;
}
</style>
