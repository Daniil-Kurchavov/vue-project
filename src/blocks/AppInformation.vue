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
          <AppPoints isGray
            >Участники, которые достигнут наибольшего прогресса и результата, станут финалистами
            конкурса</AppPoints
          >
          <AppPoints isGray
            >Победителей определяют по итогам работы с партнерами и трекерами конкурса</AppPoints
          >
        </div>
        <img class="information__card__img" src="/icons/iconsInformation/Cup.svg" alt="#" />
      </div>
      <div class="information__card">
        <h3 class="information__card__title">В чем измеряется прогресс и результат участников</h3>
        <div class="information__card__points">
          <AppPoints isGray>Договоренности о пилотировании проекта с партнерами</AppPoints>
          <AppPoints isGray>Количество внедренных решений на предприятия партнеров</AppPoints>
          <AppPoints isGray>Рост выручки проекта за время участия в конкурсе</AppPoints>
          <AppPoints isGray>Качественная доработка проекта</AppPoints>
        </div>
        <img class="information__card__img" src="/icons/iconsInformation/Computer.svg" alt="#" />
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.information {
  &__content {
    position: relative;
    margin-bottom: 210px;

    @media (max-width: 991px) {
      margin-bottom: 110px;
    }

    @media (max-width: 768px) {
      margin-bottom: 145px;
    }
  }

  &__block {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 40px;

    @media (max-width: 991px) {
      gap: 30px;
    }

    @media (max-width: 768px) {
      gap: 20px;
    }
  }

  &__title {
    max-width: 680px;
    text-align: center;

    @media (max-width: 991px) {
      max-width: 440px;
    }

    @media (max-width: 768px) {
      max-width: 360px;
    }
  }

  &__img {
    &__hands {
      position: absolute;
      top: -18%;
      transform: translateY(-50%);
      left: 5%;

      @media (max-width: 991px) {
        width: 100px;
        height: 80px;
        top: -6%;
        left: 1%;
      }

      @media (max-width: 768px) {
        width: 80px;
        height: 60px;
        top: -28%;
        left: -2%;
      }
    }
    &__rocket {
      position: absolute;
      top: 122%;
      transform: translateY(-50%);
      left: 13%;

      @media (max-width: 991px) {
        width: 100px;
        height: 120px;
        top: 103%;
        left: 4%;
      }

      @media (max-width: 768px) {
        width: 60px;
        height: 80px;
        top: 140%;
        left: 3%;
      }
    }
    &__gear {
      position: absolute;
      top: -16%;
      transform: translateY(-50%);
      right: 4%;

      @media (max-width: 991px) {
        width: 80px;
        height: 80px;
        top: -3%;
        right: 3%;
      }

      @media (max-width: 768px) {
        width: 70px;
        height: 70px;
        top: -34%;
        right: 4%;
      }
    }
    &__logo {
      position: absolute;
      top: 125%;
      transform: translateY(-50%);
      right: 14%;

      @media (max-width: 991px) {
        width: 100px;
        height: 100px;
        width: 100px;
        height: 80px;
        top: 110%;
        right: 5%;
      }

      @media (max-width: 768px) {
        width: 50px;
        height: 50px;
        top: 145%;
        right: 10%;
      }
    }
  }

  &__cards {
    display: flex;
    gap: 20px;

    @media (max-width: 991px) {
      flex-direction: column;
    }

    @media (max-width: 768px) {
      gap: 15px;
    }
  }

  &__card {
    position: relative;
    padding: 40px;
    padding-bottom: 55px;
    border: 1px solid #dee3e1;
    border-radius: 32px;
    flex: 1;
    background:
      linear-gradient(
        340deg,
        rgba(151, 255, 200, 0.8) 0%,
        rgba(151, 255, 200, 0.4) 30%,
        rgba(151, 255, 200, 0) 100%
      ),
      linear-gradient(to right, rgb(255, 255, 255) 70%, rgba(255, 255, 255, 0) 100%);
    background-blend-mode: overlay;

    @media (max-width: 991px) {
      padding: 30px;
    }

    @media (max-width: 768px) {
      padding: 20px;
      padding-bottom: 100px;
    }

    &__points {
      display: flex;
      flex-direction: column;
      gap: 20px;

      @media (max-width: 991px) {
        gap: 5px;
      }

      @media (max-width: 768px) {
        gap: 12px;
      }
    }

    &__title {
      font-size: 28px;
      margin-bottom: 32px;
      max-width: 385px;
      line-height: 100%;

      @media (max-width: 991px) {
        font-size: 24px;
        line-height: 125%;
        margin-bottom: 20px;
        max-width: 340px;
      }

      @media (max-width: 768px) {
        font-size: 18px;
        line-height: 145%;
        max-width: 245px;
      }
    }

    &__img {
      position: absolute;
      top: 73%;
      transform: translateY(-50%);
      right: 5%;

      @media (max-width: 991px) {
        top: 53%;
        right: 3%;
      }

      @media (max-width: 768px) {
        width: 120px;
        height: 100px;
        top: 83%;
        right: 7%;
      }
    }
  }
}
</style>
