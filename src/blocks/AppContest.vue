<script setup>
import AppButton from '@/components/AppButton.vue';
import AppTag from '@/components/AppTag.vue';
import AppLineIcons from '@/components/AppLineIcons.vue';
</script>

<template>
  <div class="app-contest">
    <div class="app-contest__block">
      <div class="app-contest__content">
        <AppTag class="app-contest__tag">Технологический конкурс</AppTag>
        <h1 class="title-64">5G Умный город</h1>
        <p class="app-contest__text text-16">
          Предложите свое уникальное решение в сфере технологических разработок
        </p>
        <div class="app-contest__bid">
          <AppButton class="app-contest__bid__button">Принять участие</AppButton>
          <p class="text-16 text__gray">Заявки принимаются до 27 марта</p>
        </div>
      </div>
      <div class="app-contest__image-wrapper">
        <div class="app-contest__img-content">
          <img class="app-contest__img" src="/graphics.png" alt="#" />
        </div>
      </div>
    </div>
    <AppLineIcons />
  </div>
</template>

<style scoped lang="scss">
.title-64 {
  margin-bottom: 10px;

  @media (max-width: 768px) {
    margin-bottom: 12px;
  }
}

.text__gray {
  color: $gray;
  width: 170px;

  @media (max-width: 991px) {
    padding-left: 8px;
    width: 175px;
  }

  @media (max-width: 768px) {
    width: 100%;
    padding-left: 20px;
  }
}

.app-contest {
  background-color: #ffffff;
  border-radius: 60px;
  padding-top: 60px;

  @media (max-width: 991px) {
    padding-top: 35px;
    border-radius: 24px;
  }

  @media (max-width: 768px) {
    padding-top: 25px;
  }

  &__block {
    display: flex;
    justify-content: space-between;
    margin-bottom: 85px;
    padding: 0 60px;
    gap: 30px;

    @media (max-width: 991px) {
      padding: 0 35px;
      margin-bottom: 60px;
    }

    @media (max-width: 768px) {
      flex-direction: column;
      padding: 0 28px;
      margin-bottom: 40px;
    }
  }

  &__content {
    margin-top: 50px;

    @media (max-width: 991px) {
      margin-top: -3px;
    }
  }

  &__tag {
    margin-bottom: 15px;

    @media (max-width: 991px) {
      margin-bottom: 20px;
    }

    @media (max-width: 768px) {
      margin-bottom: 15px;
    }
  }

  &__text {
    margin-bottom: 45px;
    width: 305px;

    @media (max-width: 991px) {
      margin-bottom: 30px;
    }

    @media (max-width: 768px) {
      max-width: 270px;
      margin-bottom: 20px;
    }
  }

  &__bid {
    display: flex;
    gap: 15px;

    @media (max-width: 991px) {
      flex-direction: column;
      gap: 10px;
    }

    @media (max-width: 768px) {
      gap: 15px;
    }

    &__button {
      @media (max-width: 768px) {
        align-self: stretch;
      }
    }
  }

  &__img {
    position: absolute;
    z-index: 1;
    top: 50%;
    transform: translateY(-50%);
    right: -13%;

    @media (max-width: 991px) {
      height: 100%;
      right: -20%;
    }

    @media (max-width: 768px) {
      right: -10%;
      transform: translateY(-48%);
    }
  }

  &__img-content {
    width: 100%;
    height: 100%;
    background: linear-gradient(to right, #ddf9e8, #dbf3e5);
    border-radius: 36px;
  }

  &__image-wrapper {
    position: relative;
    border-radius: 36px;
    outline: 12px solid #fff;
    width: 480px;
    height: 430px;
    box-shadow: 0 21px 69.8px 0 rgba(0, 0, 0, 0.12);
    flex-shrink: 0;

    @media (max-width: 991px) {
      width: 260px;
      height: 290px;
      outline: 6px solid #fff;
    }

    @media (max-width: 768px) {
      width: 300px;
    }
  }
}
</style>
