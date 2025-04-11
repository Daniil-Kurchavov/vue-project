<script setup>
import AppButton from '@/components/AppButton.vue';
import AppTag from '@/components/AppTag.vue';
import AppLargeTitle from '@/components/AppLargeTitle.vue';
import AppRegularText from '@/components/AppRegularText.vue';
</script>

<template>
  <div class="app-contest">
    <AppTag class="app-contest__tag" data-tete="aaaa">Технологический конкурс</AppTag>
    <AppLargeTitle />
    <AppRegularText
      >Предложите свое уникальное решение<br />в сфере технологических разработок</AppRegularText
    >
    <AppButton>Принять участие</AppButton>
    <AppRegularText class="text__opacity">Заявки принимаются до 27 марта</AppRegularText>
  </div>
</template>

<style scoped lang="scss">
.text__opacity {
  opacity: 0.4;
}

.app-contest {
  &__tag {
    margin-top: 12px;
  }
}
</style>
