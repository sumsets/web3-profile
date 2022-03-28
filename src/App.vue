<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <profile-top msg="oguz metehan" :no="1453"/>
  </div>
</template>

<script>
import ProfileTop from './components/ProfileTop.vue';
import Style from './style.scss';

export default {
  name: 'App',
  src: {
    Style,
  },
  components: {
    ProfileTop,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  width: 375px;
}
</style>
