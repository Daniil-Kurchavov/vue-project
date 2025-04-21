<script setup>
import AppTag from '@/components/AppTag.vue';
</script>

<template>
  <div class="calendar">
    <AppTag class="calendar__tag">Календарь</AppTag>
    <h2 class="calendar__title title-48">Этапы проведения конкурса</h2>
    <div class="calendar__dates">
      <!-- <p class="calendar__data">До 27 марта</p>
      <p class="calendar__data">28 марта - 2 апреля</p>
      <p class="calendar__data">3 апреля</p>
      <p class="calendar__data">4 апреля</p>
      <p class="calendar__data">16 мая</p> -->
    </div>
    <div class="calendar__content">
      <p class="calendar__data data1">До 27 марта</p>
      <p class="calendar__data data2">28 марта - 2 апреля</p>
      <p class="calendar__data data3">3 апреля</p>
      <p class="calendar__data data4">4 апреля</p>
      <p class="calendar__data data5">16 мая</p>
      <div class="calendar__card__cell cell1">
        <div class="calendar__card card-active">
          <div class="calendar__card__img img-active">
            <img class="calendar__image" src="/icons/iconsCalendar/icon1.svg" alt="#" />
          </div>
          <h3 class="calendar__card__title title-active">Приём заявок</h3>
        </div>
      </div>
      <div class="calendar__card__cell cell2">
        <div class="calendar__card">
          <div class="calendar__card__img">
            <img class="calendar__image" src="/icons/iconsCalendar/icon2.svg" alt="#" />
          </div>
          <h3 class="calendar__card__title">Экспертный отбор</h3>
        </div>
      </div>
      <div class="calendar__card__cell cell3">
        <div class="calendar__card">
          <div class="calendar__card__img">
            <img class="calendar__image" src="/icons/iconsCalendar/icon3.svg" alt="#" />
          </div>
          <h3 class="calendar__card__title">Публикация участников </h3>
        </div>
      </div>

      <div class="calendar__card__cell cell4">
        <div class="calendar__card">
          <div class="calendar__card__img">
            <img class="calendar__image" src="/icons/iconsCalendar/icon4.svg" alt="#" />
          </div>
          <h3 class="calendar__card__title">Проведение основного этапа </h3>
        </div>
      </div>
      <div class="calendar__card__cell cell5">
        <div class="calendar__card">
          <div class="calendar__card__img">
            <img class="calendar__image" src="/icons/iconsCalendar/icon5.svg" alt="#" />
          </div>
          <h3 class="calendar__card__title">Демо-день с партнерами </h3>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.calendar {
  &__tag {
    margin-bottom: 24px;
  }

  &__title {
    margin-bottom: 32px;
  }

  &__dates {
    display: flex;
    gap: 150px;
  }

  &__data {
    color: $green;
    font-size: 18px;
    line-height: 145%;
    margin: 35px 0 15px 20px;
  }

  &__content {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-areas:
      'f g k l n'
      'a . . . .'
      '. b . . .'
      '. . c . .'
      '. . . d d'
      '. . . . e';
    background:
      linear-gradient(
          90deg,
          transparent calc(20% - 0.5px),
          #E7E7E7 calc(20% - 0.5px),
          #E7E7E7 20%,
          transparent 20%
        )
        0 0 / 100% 100%,
      linear-gradient(
          90deg,
          transparent calc(40% - 0.5px),
          #E7E7E7 calc(40% - 0.5px),
          #E7E7E7 40%,
          transparent 40%
        )
        0 0 / 100% 100%,
      linear-gradient(
          90deg,
          transparent calc(60% - 0.5px),
          #E7E7E7 calc(60% - 0.5px),
          #E7E7E7 60%,
          transparent 60%
        )
        0 0 / 100% 100%,
      linear-gradient(
          90deg,
          transparent calc(80% - 0.5px),
          #E7E7E7 calc(80% - 0.5px),
          #E7E7E7 80%,
          transparent 80%
        )
        0 0 / 100% 100%;
    background-repeat: no-repeat;

  &__image {
    vertical-align: middle;
  }

  &__card {
    display: flex;
    gap: 10px;
    border: 2px dashed #e3e3e4;
    border-radius: 100px;
    align-items: center;
    padding: 8px;

    &__cell {
      padding: 0 20px;
    }

    &__img {
      min-width: 54px;
      height: 54px;
      text-align: center;
      line-height: 54px;
      background-color: #F6F6F6;
      border-radius: 100px;
    }

    &__title {
      font-size: 14px;
      line-height: 143%;
    }
  }
  .card-active {
    background-color: $light-green;
    border: none;
  }

  .img-active {
    background-color: inherit;
  }

  .title-active {
    color: $green;
  }

  .cell1 {
    grid-area: a;
    padding-left: 0;
  }
  .cell2 {
    grid-area: b;
  }
  .cell3 {
    grid-area: c;
  }
  .cell4 {
    grid-area: d;
    margin-bottom: 12px;
    position: relative;
    background-color: #ffffff;
    z-index: 1;
  }
  .cell5 {
    grid-area: e;
  }
  .data1 {
    grid-area: f;
    margin-left: 0;
  }
}
</style>
