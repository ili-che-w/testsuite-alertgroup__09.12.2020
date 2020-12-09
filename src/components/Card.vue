<template>
  <div class="card">
    <header class="card__header">
      <h1 class="card__title">Карточка квартиры</h1>
      <button class="card__close"><img alt="close"></button>
    </header>
    <div class="card__info">
      <div class="card__metrics"></div>
      <div class="card__status"></div>
    </div>
    <div class="card__tabs">
      <div class="tab tab--active">
        <div class="tab__title">Информация</div>
        <div class="tab__body">
          <Slider />
          <Pricing />
          <MicroCards />
        </div>
      </div>
      <div class="tab">
        <div class="tab__title">Площади</div>
        <div class="tab__body"></div>
      </div>
      <div class="tab">
        <div class="tab__title">Акции</div>
        <div class="tab__body"></div>
      </div>
      <div class="tab">
        <div class="tab__title">Преимущества</div>
        <div class="tab__body"></div>
      </div>
    </div>
    <footer class="card__footer">
      <ButtonsPanel />
    </footer>
  </div>
</template>

<script>
import Slider from './Slider.vue'
import Pricing from './Pricing.vue'
import MicroCards from './MicroCards.vue'
import ButtonsPanel from './ButtonsPanel.vue'

export default {
  name: 'Card',
  components: {
    Slider,
    Pricing,
    MicroCards,
    ButtonsPanel
  }
}
</script>

<style scoped>
  .card__info {
    display: flex;
    justify-content: space-between;
  }
  .tab--active ~ .tab {
    display: none;
  }
</style>