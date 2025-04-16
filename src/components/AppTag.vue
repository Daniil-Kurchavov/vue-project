<script setup></script>

<template>
  <Tag class="tag"><slot></slot></Tag>
</template>

<style scoped lang="scss">
.tag {
  height: 32px;
  background-color: rgba(0, 174, 70, 0.1);
  color: #00ae46;
  border-radius: 8px;
  font-size: 14px;
  line-height: 120%;
  display: flex;
  text-transform: uppercase;
  letter-spacing: 1px;
  text-align: center;
  align-items: center;
  width: fit-content;
  padding: 0 12px;

  @media (max-width: 991px) {
    font-size: 12px;
    padding: 0 10px;
    height: 28px;
  }

  @media (max-width: 768px) {
    line-height: 115%;
    font-size: 11px;
    height: 24px;
    border-radius: 4px;
    padding: 0 8px;
  }
}
</style>
