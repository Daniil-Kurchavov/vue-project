<script setup>
import AppTag from '@/components/AppTag.vue';
</script>

<template>
  <div class="calendar">
    <AppTag class="calendar__tag">Календарь</AppTag>
    <h2 class="calendar__title title-48">Этапы проведения конкурса</h2>
    <div class="calendar__content">
      <div class="calendar__line">
        <p class="calendar__line__data">До 27 марта</p>
        <div class="calendar__line__container__active">
          <div class="calendar__line__img__active">
            <img class="line__image" src="/icons/iconsCalendar/icon1.svg" alt="#" />
          </div>
          <h3 class="calendar__line__title__active">Приём заявок</h3>
        </div>
      </div>
      <div class="calendar__divider"></div>
      <div class="calendar__line">
        <p class="calendar__line__data">28 марта - 2 апреля</p>
        <div class="calendar__line__container">
          <div class="calendar__line__img">
            <img class="line__image" src="/icons/iconsCalendar/icon2.svg" alt="#" />
          </div>
          <h3 class="calendar__line__title">Экспертный отбор</h3>
        </div>
      </div>
      <div class="calendar__divider"></div>
      <div class="calendar__line">
        <p class="calendar__line__data">3 апреля</p>
        <div class="calendar__line__container mt150">
          <div class="calendar__line__img">
            <img class="line__image" src="/icons/iconsCalendar/icon3.svg" alt="#" />
          </div>
          <h3 class="calendar__line__title">Публикация участников</h3>
        </div>
      </div>
      <div class="calendar__divider"></div>
      <div class="calendar__line">
        <p class="calendar__line__data">4 апреля</p>
        <div class="calendar__line__container mt225">
          <div class="calendar__line__img">
            <img class="line__image" src="/icons/iconsCalendar/icon4.svg" alt="#" />
          </div>
          <h3 class="calendar__line__title">Проведение основного этапа</h3>
        </div>
      </div>
      <div class="calendar__divider"></div>
      <div class="calendar__line">
        <p class="calendar__line__data">16 мая</p>
        <div class="calendar__line__container mt305">
          <div class="calendar__line__img">
            <img class="line__image" src="/icons/iconsCalendar/icon5.svg" alt="#" />
          </div>
          <h3 class="calendar__line__title">Демо-день с партнерами</h3>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.line__image {
  vertical-align: middle;
}

.calendar {
  &__tag {
    margin-bottom: 24px;
  }

  &__title {
    margin-bottom: 68px;
  }

  &__content {
    display: flex;
    gap: 20px;
  }

  &__divider {
    width: 1px;
    height: 450px;
    background-color: #CCCCCC;
  }

  &__line {
    &__data {
      font-size: 18px;
      color: $green;
      line-height: 145%;
    }

    &__container {
      display: flex;
      padding: 8px;
      width: fit-content;
      border-radius: 100px;
      align-items: center;
      margin-top: 85px;
      border: 3px dotted #e3e3e4;
      gap: 12px;

      &__active {
        background-color: $light-green;
        display: flex;
        padding: 8px;
        border-radius: 100px;
        width: fit-content;
        align-items: center;
        margin-top: 15px;
      }
    }

    &__img {
      width: 54px;
      height: 54px;
      border-radius: 100px;
      text-align: center;
      line-height: 54px;
      background-color: #f6f6f6;

      &__active {
        width: 54px;
        height: 54px;
        border-radius: 100px;
        text-align: center;
        line-height: 54px;
      }
    }

    &__title {
      font-size: 14px;
      line-height: 143%;

      &__active {
        line-height: 143%;
        font-size: 14px;
        color: $green;
      }
    }
  }

  .mt150 {
    margin-top: 150px;
  }

  .mt225 {
    margin-top: 225px;
  }

  .mt305 {
    margin-top: 305px;
  }
}
</style>
