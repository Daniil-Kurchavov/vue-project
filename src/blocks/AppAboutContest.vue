<script setup>
import AppCardAboutContest from '@/components/AppCardAboutContest.vue';
import AppTag from '@/components/AppTag.vue';
</script>

<template>
    <div class="app-about">
        <div class="app-about__cards">
            <AppCardAboutContest>Юридическое лицо или ИП зарегистрировано в России</AppCardAboutContest>
            <AppCardAboutContest>Стадия MVP или готовое решение</AppCardAboutContest>
            <AppCardAboutContest>Готовность к запуску и пилотированию продукта с партнерами конкурса</AppCardAboutContest>
        </div>
        <div class="app-about__container">
            <AppTag class="app-about__tag">О конкурсе</AppTag>
            <h2 class="app-about__title title-48">Внедрение технологии 5G в инфраструктуру</h2>
            <h3 class="app-about__subtitle title-18">Цели конкурса</h3>
            <div class="app-about__goal">
                <p class="text-16">Выявление и внедрение инновационных продуктов</p>
                <p class="text-16">Улучшение беспроводной связи пятого поколения</p>
                <p class="text-16">Поддержание развития цифровых технологий</p>
                <p class="text-16">Систематизация направлений применения сетей 5G</p>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
    .app-about {
        display: flex;
        padding: 60px;
        border-radius: 48px;
        box-shadow: 0 10px 48px 0 rgba(0, 0, 0, 0.12);
        gap: 90px;

        &__cards {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        &__tag {
            margin-bottom: 24px;
        }

        &__title {
            margin-bottom: 40px;
        }

        &__subtitle {
                margin-bottom: 16px;
            }

        &__goal {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }
    }
</style>