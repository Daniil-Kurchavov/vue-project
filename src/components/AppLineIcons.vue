<script setup></script>

<template>
  <div class="divider-icons__container">
    <div class="divider-icons__agent"><img src="/moscow_agent.svg" alt="#" /></div>
    <div class="divider"></div>
    <div class="divider-icons__project"><img src="/moscow-project.svg" alt="#" /></div>
    <div class="divider"></div>
    <div class="divider-icons__teh"><img src="/teh.svg" alt="#" /></div>
  </div>
</template>

<style lang="scss">
.divider {
  width: 1px;
  height: 75px;
  background-color: #1C1D22;
  opacity: 0.1;
}

.divider-icons__container {
  display: flex;
  align-items: center;
  margin-bottom: 60px;
  justify-content: space-around;
}

.divider-icons__agent {
  width: 180px;
  height: 60px;

  & img {
    width: 100%;
    height: 100%;
  }
}

.divider-icons__project {
  width: 120px;
  height: 60px;

  & img {
    width: 100%;
    height: 100%;
  }
}

.divider-icons__teh {
  width: 312px;
  height: 60px;

  & img {
    width: 100%;
    height: 100%;
  }
}
</style>
