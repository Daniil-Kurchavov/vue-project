<script setup>
defineProps({
  isGray: Boolean,
});
</script>

<template>
  <div class="points">
    <p class="points__line"></p>
    <p class="text-16" :class="isGray && 'gray'"><slot></slot></p>
  </div>
</template>

<style lang="scss">
.points {
  display: flex;
  align-items: center;
  gap: 13px;

  @media (max-width: 991px) {
    gap: 8px;
    align-items: normal;
  }

  @media (max-width: 768px) {
    gap: 15px;
  }

  &__line {
    width: 8px;
    height: 2px;
    background-color: $green;

    @media (max-width: 991px) {
      margin-top: 8px;
    }
  }
}
</style>
