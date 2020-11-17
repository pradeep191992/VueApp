<template>
  <div class="header">
    <H1>Header Component</H1>
    <Navigation />
  </div>
</template>

<script>
import Navigation from "./../navigation/navigation.vue";
export default {
  name: "Header",
  components: {
    Navigation
  }
};
</script>

<style lang="scss" scoped>
</style>