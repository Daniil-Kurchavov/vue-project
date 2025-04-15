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
          <AppButton>Принять участие</AppButton>
          <p class="text-16 text__opacity">Заявки принимаются до 27 марта</p>
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
}

.text__opacity {
  color: $gray;
  width: 170px;
  line-height: 150%;
}

.app-contest {
  background-color: #ffffff;
  border-radius: 60px;
  padding-top: 60px;
  
  &__block {
    display: flex;
    justify-content: space-between;
    margin-bottom: 80px;
    padding: 0 60px;
  }

  &__content {
    margin-top: 45px;
  }

  &__tag {
    margin-bottom: 15px;
  }

  &__text {
    margin-bottom: 50px;
    width: 305px;
    line-height: 150%;
  }

  &__bid {
    display: flex;
    gap: 15px;
  }

  &__img {
    position: absolute;
    z-index: 1;
    top: 50%;
    transform: translateY(-50%);
    right: -13%;
  }

  &__img-content {
    width: 100%;
    height: 100%;
    background: linear-gradient(to right, #ddf9e8, #DBF3E5);
    border-radius: 36px;
  }

  &__image-wrapper {
    position: relative;
    border-radius: 36px;
    outline: 12px solid #fff;
    width: 480px;
    height: 430px;
    box-shadow: 0 21px 69.8px 0 rgba(0, 0, 0, 0.12);
  }
}
</style>
