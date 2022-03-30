<template>
  <div div v-if="degree === 0">{{ degree }}</div>
  <div v-else>{{ degree }}</div>
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
