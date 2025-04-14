<script setup></script>

<template>
  <div class="line-icons__container">
    <div class="line-icons__agent"><img src="./../../public/moscow_agent.svg" alt="#" /></div>
    <div class="line"></div>
    <div class="line-icons__project"><img src="./../../public/moscow-project.svg" alt="#" /></div>
    <div class="line"></div>
    <div class="line-icons__teh"><img src="./../../public/teh.svg" alt="#" /></div>
  </div>
</template>

<style lang="scss">
.line-icons__container {
  margin-bottom: 60px;
}

.line {
  width: 1px;
  height: 75px;
  background-color: #1C1D22;
  opacity: 0.1;
}

.line-icons__container {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.line-icons__agent {
  width: 138px;
  height: 45px;

  & img {
    width: 100%;
    height: 100%;
  }
}

.line-icons__project {
  width: 92px;
  height: 45px;

  & img {
    width: 100%;
    height: 100%;
  }
}

.line-icons__teh {
  width: 244px;
  height: 45px;

  & img {
    width: 100%;
    height: 100%;
  }
}
</style>
