<template>
  <img v-if="degree === 0" src="@/assets/Wifi2.svg" alt="wifi0">
  <img v-else-if="degree === 1" src="@/assets/Wifi1.svg" alt="wifi1">
  <img v-else-if="degree === 2" src="@/assets/Wifi2.svg" alt="wifi2">
  <img v-else src="@/assets/Wifi3.svg" alt="wifi3">
</template>

<script>
export default {
  props: {
    degree: Number,
  },
};
</script>
