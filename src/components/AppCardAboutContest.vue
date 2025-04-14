<script setup></script>

<template>
    <div class="app-card-about">
        <div class="app-card-about__img"></div>
        <div class="app-card-about__text text-16"><slot></slot></div>
    </div>
</template>

<style lang="scss">
    .app-card-about {
        display: flex;
        border-radius: 100px;
        border:1px solid rgb(28, 29, 34, 0.1);
        align-items: center;
        width: 460px;
        gap: 32px;
        padding: 8px;
        

        &__img {
            width: 160px;
            height: 95px;
            background: linear-gradient(to right, #DDF9E8, rgba(0, 174, 70, 0.3));
            border-radius: 100px;
            flex: none;
        }

        &__text {
            font-family: "TTFirsNeue-Medium";
            line-height: 24px;
            color: #000000;
        }
    }


</style>