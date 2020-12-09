<template>
  <div class="slider">
    <div class="slider__tabs">
      <div class="slider__tab">
        <a href="#" class="slider__link">
          <img alt="image">
        </a>
      </div>
    </div>
    <div class="slider__switch">
      <span class="slider-switch__item"></span>
    </div>
  </div>
</template>

<style lang="scss">
  @import '@/assets/variables.scss';

  .slider__switch {
    display: flex;
    justify-content: space-around;
  }
  .slider-switch__item {
    display: inline-block;
    background-color: $accent;
    height: 4px;
    width: 4px;
    border-radius: 2px;
  }
</style>