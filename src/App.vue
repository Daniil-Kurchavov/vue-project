<script setup>
import AppContest from './blocks/AppContest.vue';
import AppAboutContest from './blocks/AppAboutContest.vue';
</script>

<template>
  <div class="page-contest container">
    <AppContest class="page-contest__first-screen" />
    <AppAboutContest />
  </div>
</template>

<style scoped lang="scss">
.page-contest {
  &__first-screen {
    margin-bottom: 60px;

    @media (max-width: 991px) {
      margin-bottom: 65px;
    }
  }
}
.container {
  width: 1280px;
  margin: 0 auto;
  padding: 0 20px;
  position: relative;
  max-width: 100%;

  @media (max-width: 991px) {
    width: 745px;
  }
}
</style>
