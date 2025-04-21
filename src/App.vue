<script setup>
import AppContest from './blocks/AppContest.vue';
import AppAboutContest from './blocks/AppAboutContest.vue';
import AppPossibilities from './blocks/AppPossibilities.vue';
import AppInformation from './blocks/AppInformation.vue';
import AppCalendarNew from './blocks/AppCalendar.vue';
</script>

<template>
  <div class="page-contest container">
    <AppContest class="page-contest__first-screen" />
    <AppAboutContest class="page-contest__second-screen" />
    <AppPossibilities class="page-contest__third-screen" />
    <AppInformation class="page-contest__fourth-screen"/>
    <AppCalendarNew />
  </div>
</template>

<style scoped lang="scss">
.page-contest {
  &__first-screen {
    margin-bottom: 60px;

    @media (max-width: 991px) {
      margin-bottom: 65px;
    }

    @media (max-width: 768px) {
      margin-bottom: 45px;
    }
  }

  &__second-screen {
    margin-bottom: 120px;
  }

  &__third-screen {
    margin-bottom: 235px;

    @media (max-width: 991px) {
      margin-bottom: 110px;
    }
  }

  &__fourth-screen {
    margin-bottom: 120px;
  }
}

.container {
  width: 1280px;
  margin: 0 auto;
  padding: 0 20px;
  position: relative;
  max-width: 100%;
  background-color: #ffffff;
  border-radius: 60px;

  @media (max-width: 991px) {
    width: 745px;
  }

  @media (max-width: 768px) {
    width: 375px;
    padding: 0 20px;
  }
}
</style>
