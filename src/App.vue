<template>
  <div id="app">
    <b-container>
      <profile-top />
    </b-container>
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
}
</style>
