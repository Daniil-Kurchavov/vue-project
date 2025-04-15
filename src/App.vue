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
  }
}

.container {
  width: 1280px;
  margin: 0 auto;
  padding: 0 20px;
  position: relative;
}
</style>
