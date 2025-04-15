<script setup></script>

<template>
  <button class="button"><slot></slot></button>
</template>

<style scoped lang="scss">
.button {
  padding: 12px 25px;
  background: linear-gradient(to right, #14d461, #12acdd);
  border-radius: 12px;
  color: $white;

  @media (max-width:991px) {
    padding: 15px 25px;
  }
}
</style>
