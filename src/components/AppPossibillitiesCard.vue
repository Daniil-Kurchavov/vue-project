<script setup>
defineProps({
  imageSrc: {
    type: String,
  },
  secondaryImageSrc: {
    type: String,
    default: null,
  },
  title: {
    type: String,
  },
  text: {
    type: String,
  },
  gridNum: {
    type: String,
  },
});
</script>

<template>
  <div :class="'possibilities-card possibilities-card' + gridNum">
    <div class="possibilities-card__flex">
      <div class="possibilities-card__block">
        <img class="possibilities-card__img" :src="imageSrc" alt="#" />
      </div>
      <h3 class="possibilities-card__title">{{ title }}</h3>
    </div>
    <p class="possibilities-card__text">{{ text }}</p>
    <img
      v-if="secondaryImageSrc"
      class="possibilities-card__secondary-img"
      :src="secondaryImageSrc"
      alt="#"
    />
  </div>
</template>

<style lang="scss">
.possibilities-card {
  padding: 28px;
  padding-bottom: 5px;
  border-radius: 24px;
  border: 1px solid #e3e3e4;
  position: relative;

  @media (max-width: 991px) {
    padding: 22px;
  }

  @media (max-width: 768px) {
    padding: 20px;
    padding-bottom: 5px;
  }

  &__flex {
    @media (max-width: 768px) {
      display: flex;
      gap: 15px;
    }
  }

  &__block {
    position: relative;
    height: 44px;
    width: 44px;
    background-color: $light-green;
    border-radius: 8px;
    margin-bottom: 38px;

    @media (max-width: 991px) {
      margin-bottom: 24px;
    }
  }

  &__img {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    right: 20%;
  }

  &__title {
    font-size: 24px;
    line-height: 133%;
    color: $primary-dark;
    max-width: 255px;
    margin-bottom: 8px;

    @media (max-width: 991px) {
      font-size: 22px;
      line-height: 100%;
      max-width: 281px;
      margin-bottom: 9px;
    }

    @media (max-width: 768px) {
      font-size: 18px;
      line-height: 145%;
      max-width: 224px;
    }
  }

  &__text {
    max-width: 230px;
    font-size: 16px;
    color: $primary-dark;
    font-family: 'TTFirsNeue-Regular';
    line-height: 150%;

    @media (max-width: 991px) {
      line-height: 120%;
      max-width: 285px;
    }
  }

  &__secondary-img {
    position: absolute;
    top: 63%;
    transform: translateY(-50%);
    right: -4%;

    @media (max-width: 991px) {
      right: 4%;
      width: 36%;
      top: 55%;
    }

    @media (max-width: 768px) {
      top: 73%;
      right: 26%;
      width: 60%;
      height: 59%;
    }
  }
}
</style>
