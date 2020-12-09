<template>
  <div class="card">
    <header class="card__top">
      <CardHeader />
      <div class="container">
        <CardInfo />
      </div>
    </header>
    <div class="container">
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
    </div>
    <footer class="card__footer">
      <ButtonsPanel />
    </footer>
  </div>
</template>

<script>
import CardHeader from '@/components/CardHeader.vue'
import CardInfo from '@/components/CardInfo.vue'
import Slider from '@/components/Slider.vue'
import Pricing from '@/components/Pricing.vue'
import MicroCards from '@/components/MicroCards.vue'
import ButtonsPanel from '@/components/ButtonsPanel.vue'

export default {
  name: 'Card',
  components: {
    CardHeader,
    CardInfo,
    Slider,
    Pricing,
    MicroCards,
    ButtonsPanel
  }
}
</script>

<style lang="scss">
  @import '@/assets/variables.scss';

  .card__top {
    width: 100%;
    background-color: $white;
  }

  .container {
    width: $mobile-md - 16px;
    margin: 0 auto;
    @media (max-width: $mobile-md - 1) {
      width: auto;
      padding: 0 8px;
    }
  }

  .tab--active ~ .tab {
    display: none;
  }
</style>