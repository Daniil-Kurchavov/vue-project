<script setup>
import AppButton from '@/components/AppButton.vue';
import AppTag from '@/components/AppTag.vue';
import AppLargeTitle from '@/components/AppLargeTitle.vue';
import AppRegularText from '@/components/AppRegularText.vue'
</script>

<template>
  <AppTag>Технологический конкурс</AppTag>
  <AppLargeTitle />
  <AppRegularText>Предложите свое уникальное решение<br>в сфере технологических разработок</AppRegularText>
  <AppButton>Принять участие</AppButton>
  <AppRegularText class="text__opacity">Заявки принимаются до 27 марта</AppRegularText>
</template>

<style scoped lang="scss">
    .text__opacity {
        opacity: 0.4;
    }
</style>
