<template>
  <div class="card-info">
    <div class="card-info__metrics">
      <div class="metrics-item">
        <span class="metrics-item__text">
          №12
        </span>
      </div>
      <div class="metrics-item">
        <span class="metrics-item__caption">М</span>
        <span class="metrics-item__text">
          59.52м²
        </span>
      </div>
    </div>
    <div class="card-info__status">
      Свободно
    </div>
  </div>
</template>

<style lang="scss">
  @import '@/assets/variables.scss';

  .card-info {
    @include flex-space-between;
    text-align: center;
    height: 48px;
    &__metrics {
      display: flex;
    }
    &__status {
      background-color: $green-50;
      height: 24px;
      width: 80px;
      padding: 0 10px;
      border-radius: 32px;
      font-size: 12px;
      line-height: 24px;
      color: $white;
    }
  }
  .metrics-item {
    border: 1px solid $gray-60;
    border-radius: 3px;
    font-size: 14px;
    font-weight: 700;
    line-height: 30px;
    color: $black;
    & + & {
      margin-left: 4px;
    }
    &__caption, &__text {
      display: inline-block;
      padding: 0 8px;
    }
    &__caption {
      border-right: 1px solid $gray-60;
      padding-right: 6px;
    }
  }
</style>
