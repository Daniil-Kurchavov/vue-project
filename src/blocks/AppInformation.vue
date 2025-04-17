<script setup>
import AppButton from '@/components/AppButton.vue';
import AppPoints from '@/components/AppPoints.vue';
</script>

<template>
  <div class="information">
    <div class="information__content">
      <div class="information__block">
        <h2 class="information__title title-48">
          Подайте заявку до 27 марта и станьте победителем
        </h2>
        <div class="information__button"><AppButton>Принять участие</AppButton></div>
      </div>
      <img class="information__img__hands" src="/icons/iconsInformation/Hands.svg" alt="#" />
      <img class="information__img__rocket" src="/icons/iconsInformation/Rocket.svg" alt="#" />
      <img class="information__img__gear" src="/icons/iconsInformation/Gear.svg" alt="#" />
      <img class="information__img__logo" src="/icons/iconsInformation/Logo.svg" alt="#" />
    </div>
    <div class="information__cards">
      <div class="information__card">
        <h3 class="information__card__title">Как определяют победителей конкурса</h3>
        <div class="information__card__points">
          <AppPoints
            >Участники, которые достигнут наибольшего прогресса и результата, станут финалистами
            конкурса</AppPoints
          >
          <AppPoints
            >Победителей определяют по итогам работы с партнерами и трекерами конкурса</AppPoints
          >
        </div>
      </div>
      <div class="information__card">
        <h3 class="information__card__title">В чем измеряется прогресс и результат участников</h3>
        <div class="information__card__points">
          <AppPoints>Договоренности о пилотировании проекта с партнерами</AppPoints>
          <AppPoints>Количество внедренных решений на предприятия партнеров</AppPoints>
          <AppPoints>Рост выручки проекта за время участия в конкурсе</AppPoints>
          <AppPoints>Качественная доработка проекта</AppPoints>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.information {
  &__content {
    position: relative;
    margin-bottom: 210px;
  }

  &__block {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 40px;
  }

  &__title {
    max-width: 680px;
    text-align: center;
  }

  &__img {
    &__hands {
      position: absolute;
      top: -18%;
      transform: translateY(-50%);
      left: 5%;
    }
    &__rocket {
      position: absolute;
      top: 122%;
      transform: translateY(-50%);
      left: 13%;
    }
    &__gear {
      position: absolute;
      top: -16%;
      transform: translateY(-50%);
      right: 4%;
    }
    &__logo {
      position: absolute;
      top: 125%;
      transform: translateY(-50%);
      right: 14%;
    }
  }

  &__cards {
    display: flex;
    gap: 20px;
  }

  &__card {
    padding: 40px;
    padding-bottom: 60px;
    border: 1px solid #dee3e1;
    border-radius: 32px;
    flex: 1;

    &__points {
      display: flex;
      flex-direction: column;
      gap: 12px;
      max-width: 320px;
    }

    &__title {
      font-size: 28px;
      margin-bottom: 32px;
      max-width: 385px;
      line-height: 100%;
    }
  }
}
</style>
