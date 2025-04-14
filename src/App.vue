<script setup>
import AppContest from './blocks/AppContest.vue';
import AppAboutContest from './blocks/AppAboutContest.vue';
</script>

<template>
  <div class="container">
    <AppContest />
    <AppAboutContest />
  </div>
</template>

<style scoped lang="scss">
.container {
  width: 1280px;
  margin: 0 auto;
  padding: 0 20px;
}
</style>
