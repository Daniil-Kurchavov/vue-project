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
  grid_num: {
    type: String,
  },
  isFirstOrLast: {
    type: Boolean,
    default: false,
  },
});
</script>

<template>
  <div :class="'possibillities-card possibillities-card' + grid_num">
    <div class="possibillities-card__block">
      <img class="possibillities-card__img" :src="imageSrc" alt="#" />
    </div>
    <h3 class="possibillities-card__title">{{ title }}</h3>
    <p class="possibillities-card__text text-16">{{ text }}</p>
    <img
      v-if="isFirstOrLast && secondaryImageSrc"
      class="possibillities-card__secondary-img"
      :src="secondaryImageSrc"
      alt="#"
    />
  </div>
</template>

<style lang="scss">
.possibillities {
  &-card {
    padding: 28px;
    border-radius: 24px;
    border: 1px solid #e3e3e4;
    position: relative;

    &__block {
      position: relative;
      height: 44px;
      width: 44px;
      background-color: $light-green;
      border-radius: 8px;
      margin-bottom: 40px;
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
      margin-bottom: 12px;
    }

    &__text {
      max-width: 230px;
    }

    &__secondary-img {
      position: absolute;
      top: 52%;
      transform: translateY(-50%);
      right: -2%;
    }
  }
}
</style>
