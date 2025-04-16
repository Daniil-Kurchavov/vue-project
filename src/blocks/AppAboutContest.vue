<script setup>
import AppTag from '@/components/AppTag.vue';
import AppPoints from '@/components/AppPoints.vue';
</script>

<template>
  <div class="contest-about">
    <div class="contest-about__cards">
      <div class="contest-about__card">
        <div class="contest-about__card__img">
          <img class="card-img1" src="/icons/icon1.svg" alt="#" />
        </div>
        <p class="contest-about__card__text text-16-med">
          Юридическое лицо или&nbsp;ИП зарегистрировано в&nbsp;России
        </p>
      </div>
      <div class="contest-about__card">
        <div class="contest-about__card__img">
          <img class="card-img2" src="/icons/icon2.svg" alt="#" />
        </div>
        <p class="contest-about__card__text contest-about__card__text_min text-16-med">
          Стадия MVP или готовое решение
        </p>
      </div>
      <div class="contest-about__card">
        <div class="contest-about__card__img contest-about__card__img_cut">
          <img class="card-img3" src="/icons/icon3.svg" alt="#" />
        </div>
        <p class="contest-about__card__text text-16-med">
          Готовность к&nbsp;запуску и&nbsp;пилотированию продукта с&nbsp;партнерами конкурса
        </p>
      </div>
    </div>
    <div class="contest-about__content">
      <AppTag class="contest-about__tag">О конкурсе</AppTag>
      <h2 class="contest-about__title title-48">Внедрение технологии 5G&nbsp;в инфраструктуру</h2>
      <h3 class="contest-about__subtitle title-18">Цели конкурса</h3>
      <div class="contest-about__goal">
        <AppPoints>Выявление и&nbsp;внедрение инновационных продуктов</AppPoints>
        <AppPoints>Улучшение беспроводной связи пятого поколения</AppPoints>
        <AppPoints>Поддержание развития цифровых технологий</AppPoints>
        <AppPoints>Систематизация направлений применения сетей 5G</AppPoints>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.horizontal__line {
  width: 8px;
  height: 2px;
  background-color: $green;
}

.contest-about {
  display: flex;
  padding: 60px;
  border-radius: 48px;
  box-shadow: 0 10px 48px 0 rgba(0, 0, 0, 0.12);
  gap: 95px;

  @media (max-width: 991px) {
    flex-direction: column-reverse;
    padding: 35px;
    gap: 32px;
  }

  @media (max-width: 768px) {
    box-shadow: none;
    padding: 10px 12px;
    gap: 20px;
  }

  &__cards {
    display: flex;
    flex-direction: column;
    gap: 15px;
    flex-basis: 470px;
    flex-shrink: 0;

    @media (max-width: 991px) {
      flex-direction: row;
      height: 75px;
      overflow-x: scroll;
      overflow-y: hidden;
    }

    @media (max-width: 768px) {
      overflow-x: hidden;
      flex-direction: column;
      height: auto;
      gap: 8px;
    }
  }

  &__card {
    display: flex;
    border-radius: 100px;
    border: 1px solid rgb(28, 29, 34, 0.1);
    align-items: center;
    gap: 32px;
    padding: 8px;
    width: fit-content;

    @media (max-width: 991px) {
      width: 330px;
      flex-shrink: 0;
      gap: 10px;
      padding: 8px;
      padding-right: 15px;

      @media (max-width: 768px) {
        gap: 15px;
      }
    }

    &__img {
      position: relative;
      width: 160px;
      height: 95px;
      background: linear-gradient(to right, #ddf9e8, rgba(0, 174, 70, 0.3));
      border-radius: 100px;
      flex: none;

      @media (max-width: 991px) {
        height: 60px;
        width: 90px;
      }

      @media (max-width: 768px) {
        width: 65px;
        height: 50px;
      }

      & img {
        position: absolute;
        top: 50%;
        transform: translateY(-50%);
        width: 100%;
      }

      &_cut {
        overflow: hidden;
      }
    }

    &__text {
      font-family: 'TTFirsNeue-Medium';
      line-height: 150%;
      color: #000000;

      &_min {
        max-width: 150px;
      }
    }
  }

  &__tag {
    margin-bottom: 25px;

    @media (max-width: 991px) {
      margin-bottom: 15px;
    }

    @media (max-width: 768px) {
      margin-bottom: 15px;
    }
  }

  &__title {
    margin-bottom: 40px;

    @media (max-width: 991px) {
      max-width: 355px;
      margin-bottom: 15px;
    }
  }

  &__subtitle {
    margin-bottom: 13px;
    line-height: 145%;

    @media (max-width: 768px) {
      margin-bottom: 15px;
      line-height: 150%;
    }
  }

  &__goal {
    display: flex;
    flex-direction: column;
    gap: 13px;

    @media (max-width: 768px) {
      gap: 12px;
    }
  }

  &__line {
    display: flex;
    align-items: center;
    gap: 13px;
  }

  .card-img1 {
    transform: translateY(-63%);
  }

  .card-img2 {
    transform: translateY(-70%);
    left: -2%;
  }

  .card-img3 {
    transform: translateY(-47%);
    left: 12%;
    overflow: hidden;
  }
}
</style>
