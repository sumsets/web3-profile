<template>
  <div v-if="degree === 0"><img src="@/assets/Wifi2.svg" alt="wifi0"></div>
  <div v-else-if="degree === 1"><img src="@/assets/Wifi1.svg" alt="wifi1"></div>
  <div v-else-if="degree === 2"><img src="@/assets/Wifi2.svg" alt="wifi2"></div>
  <div v-else-if="degree === 3"><img src="@/assets/Wifi3.svg" alt="wifi3"></div>
</template>

<script>
export default {
  props: {
    degree: Number,
  },
};
</script>

<style lang="scss" scoped>
</style>
