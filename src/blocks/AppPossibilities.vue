<script setup>
import AppTag from '@/components/AppTag.vue';
import AppPossibillitiesCard from '@/components/AppPossibillitiesCard.vue';
import { ref } from 'vue';

const data = ref([
  {
    image: '/icons/iconsPossibilities/Rocket.svg',
    title: 'Создание совместных проектов',
    text: 'с другими участниками конкурса, а также партнёрами Фонда МИК',
    gridNum: '1',
    secondaryImageSrc: './icons/iconsPossibilities/big-books.svg',
  },
  {
    image: '/icons/iconsPossibilities/Hands.svg',
    title: 'Пилотирование продукта ',
    text: 'с партнерами конкурса на предприятиях крупнейших компаний в отрасли',
    gridNum: '2',
  },
  {
    image: '/icons/iconsPossibilities/Lightbulb.svg',
    title: 'PR-поддержку ',
    text: 'и повышение узнаваемости проекта от Московского инновационного кластера',
    gridNum: '3',
  },
  {
    image: '/icons/iconsPossibilities/User.svg',
    title: 'Экспертную оценку и диагностику решения ',
    text: 'от ведущих специалистов в отрасли медиа',
    gridNum: '4',
  },
  {
    image: '/icons/iconsPossibilities/Hand-coins.svg',
    title: 'Инвестиции от партнеров Фонда МИК',
    text: 'если их заинтересует решение или проект конкурсанта',
    gridNum: '5',
  },
  {
    image: '/icons/iconsPossibilities/Logo.svg',
    title: 'Возможность внедрения и масштабирования',
    text: 'проекта, если оно соответствует запросам партнеров конкурса',
    gridNum: '6',
    secondaryImageSrc: './icons/iconsPossibilities/big-logo.svg',
  },
]);
</script>

<template>
  <div class="possibilities">
    <AppTag class="possibilities__tag">Возможности</AppTag>
    <h2 class="possibilities__title title-48">Что получают участники конкурса</h2>
    <div class="possibilities__cards">
      <AppPossibillitiesCard
        v-for="(card, index) in data"
        :secondaryImageSrc="card.secondaryImageSrc"
        :key="index"
        :image-src="card.image"
        :title="card.title"
        :text="card.text"
        :gridNum="card.gridNum"
        :is-first-or-last="card.isFirstOrLast"
      />
    </div>
  </div>
</template>

<style lang="scss">
.possibilities {
  &__tag {
    margin-bottom: 24px;

    @media (max-width: 991px) {
      margin-bottom: 20px;
    }

    @media (max-width: 768px) {
      margin-bottom: 15px;
    }
  }

  &__title {
    margin-bottom: 32px;

    @media (max-width: 991px) {
      margin-bottom: 32px;
    }

    @media (max-width: 768px) {
      margin-bottom: 20px;
    }
  }

  &__cards {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-template-rows: repeat(2, 1fr);
    gap: 20px;
    grid-template-areas:
      'a a b c'
      'd f e e';

    @media (max-width: 991px) {
      grid-template-columns: repeat(2, 1fr);
      grid-template-areas:
        'a b'
        'a c'
        'd f'
        'e e';

      gap: 16px;
    }

    @media (max-width: 768px) {
      grid-template-columns: repeat(1, 1fr);
      grid-template-rows: repeat(8, 1fr);
      grid-template-areas:
        'a'
        'a'
        'b'
        'c'
        'd'
        'f'
        'e'
        'e';
        gap: 12px;
    }
  }

  &-card1 {
    grid-area: a;
  }
  &-card2 {
    grid-area: b;
  }
  &-card3 {
    grid-area: c;
  }
  &-card4 {
    grid-area: d;
  }
  &-card5 {
    grid-area: f;
  }
  &-card6 {
    grid-area: e;
  }
}
</style>
