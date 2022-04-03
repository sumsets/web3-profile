<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <profile-top msg="oguz metehan" :no="1453"/>
  </div>
</template>

<script>
import ProfileTop from './components/ProfileTop.vue';
import './style.scss';

export default {
  name: 'App',
  components: {
    ProfileTop,
  },
};
</script>

<style lang="scss">
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
  background-color: rgb(233, 225, 216);
}
</style>
