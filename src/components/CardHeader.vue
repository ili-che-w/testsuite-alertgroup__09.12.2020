<template>
  <header class="card__header">
    <h1 class="card__title">Карточка квартиры</h1>
    <div class="btn-close__wrapper">
      <button class="btn-close">
        <img src="./../assets/icons/close.svg" alt="close">
      </button>
    </div>
  </header>
</template>

<style lang="scss">
  @import '@/assets/variables.scss';

  .card__header {
    position: relative;
    @include flex-space-between;
    height: 60px;
    background-color: $white;
    box-shadow: 0px 4px 10px rgba(10, 61, 128, 0.05);
  }
  .card__title {
    margin-left: 16px;
    color: $black;
    font-size: 18px;
    font-weight: 700;
    line-height: 25px;
    text-transform: uppercase;
  }
  .btn-close__wrapper {
    height: 36px;
    width: 60px;
    display: flex;
    border-left: 1px solid $gray-60;
  }
  .btn-close {
    height: 9px;
    width: 9px;
    padding: 0;
    margin: auto;
  }
</style>