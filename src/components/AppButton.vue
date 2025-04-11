<script setup></script>

<template>
  <button class="button"><slot></slot></button>
</template>

<style scoped lang="scss">
.button {
  padding: 12px 24px;
  background: linear-gradient(to right, #14d461, #12acdd);
  border-radius: 12px;
  color: $white;
}
</style>
