<script setup></script>

<template>
  <button class="button"><slot></slot></button>
</template>

<style scoped lang="scss">
.button {
  padding: 14px 25px;
  background: linear-gradient(to right, #14d461, #12acdd);
  border-radius: 12px;
  color: $white;
  align-self: start;

  @media (max-width:991px) {
    padding: 15px 25px;
  }
}
</style>
