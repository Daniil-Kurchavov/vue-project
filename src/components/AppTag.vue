<script setup></script>

<template>
  <Tag class="tag"><slot></slot></Tag>
</template>

<style scoped lang="scss">
.tag {
  padding: 11px 12px;
  background-color: rgba($green, 0.1);
  color: $green;
  border-radius: 8px;
  font-size: 14px;
  line-height: 120%;
  display: inline-block;
  text-transform: uppercase;
}
</style>
