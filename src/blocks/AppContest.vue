<script setup>
import AppButton from '@/components/AppButton.vue';
import AppTag from '@/components/AppTag.vue';
import AppLineIcons from '@/components/AppLineIcons.vue';
</script>

<template>
  <div class="app-contest">
    <div class="app-contest__container">
      <AppTag class="app-contest__tag">Технологический конкурс</AppTag>
      <h1 class="title-64">5G Умный город</h1>
      <p class="app-contest__text text-16">
        Предложите свое уникальное решение<br />в сфере технологических разработок
      </p>
      <div class="app-contest__bid">
        <AppButton>Принять участие</AppButton>
        <p class="text-16 text__opacity">Заявки принимаются<br />до 27 марта</p>
      </div>
    </div>
    <div class="app-contest__white-border"><img class="img" src="./../../public/graphics.png" alt="#" /><div class="app-contest__img"></div></div>
  </div>
  <AppLineIcons />
</template>

<style scoped lang="scss">
.title-64 {
  margin-bottom: 16px;
}

.text__opacity {
  opacity: 0.4;
}

.app-contest {
  display: flex;
  justify-content: space-between;
  margin-bottom: 80px;

  img {
    position: absolute;
    z-index: 1;
    top: 50%;
    transform: translateY(-50%);
  }

  &__tag {
    margin-bottom: 24px;
  }

  &__text {
    margin-bottom: 48px;
  }

  &__bid {
    display: flex;
    gap: 16px;
  }

  &__img {
    width: 100%;
    height: 100%;
    background: linear-gradient(to right, #ddf9e8, rgba(0, 174, 70, 0.4));
    border-radius: 36px;
  }

  &__white-border {
    position: relative;
    background-color: #ffffff;
    border-radius: 36px;
    outline: 12px solid #fff;
    width: 500px;
    height: 450px;
    box-shadow: 0 21px 69.8px 0 rgba(0, 0, 0, 0.12);
  }
}
</style>
