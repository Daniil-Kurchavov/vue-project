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
  background-color: #1c1d22;
  opacity: 0.1;

  @media (max-width:991px) {
    height: 45px;
  }

  @media (max-width: 768px) {
    display: none;
  }
}

.divider-icons__container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 60px;

  @media (max-width: 991px) {
    padding: 0 15px;
  }

  @media (max-width: 768px) {
    padding: 0 25px;
  }
}

.divider-icons__agent {
  width: 180px;
  height: 60px;

  & img {
    width: 100%;
    height: 100%;
  }

  @media (max-width: 991px) {
    width: 140px;
    height: 45px;
  }

  @media (max-width: 768px) {
    width: 85px;
    height: 27px;
  }
}

.divider-icons__project {
  width: 120px;
  height: 60px;

  & img {
    width: 100%;
    height: 100%;
  }

  @media (max-width:991px) {
    width: 90px;
    height: 45px;
  }

  @media (max-width: 768px) {
    width: 55px;
    height: 27px;
  }
}

.divider-icons__teh {
  width: 312px;
  height: 60px;

  & img {
    width: 100%;
    height: 100%;
  }

  @media (max-width:991px) {
    width: 240px;
    height: 45px;
  }

  @media (max-width: 768px) {
    width: 125px;
    height: 23px;
  }
}
</style>
