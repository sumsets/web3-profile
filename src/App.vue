<template>
  <div id="app">
    <b-container>
      <profile-top />
      <courses-section />
    </b-container>
  </div>
</template>

<script>
import ProfileTop from './components/ProfileTop.vue';
import CoursesSection from './components/CoursesSection.vue';
import './style.scss';

export default {
  name: 'App',
  components: {
    ProfileTop,
    CoursesSection,
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
