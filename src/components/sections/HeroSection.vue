<script setup>
import HeroButton from '../ui/HeroButton.vue'
</script>

<template>
  <div id="hero" class="hero">
    <div class="inner-wrap">
      <p class="text-accent">Paradise Garden</p>
      <h1>Professional Garden Maker</h1>
      <p>is our Perfect Dream</p>
      <HeroButton>Free Quote</HeroButton>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.hero {
  background: url('@/assets/images/premium_photo-1679864498164-253f0261b9fa.jpeg');
  background-size: cover;
  background-repeat: no-repeat;

  .inner-wrap {
    background: rgba(0, 0, 0, 0.5);
    width: 100%;
    height: 100%;
    color: var(--text-on-dark-background);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    text-align: center;
    gap: 16px;
  }

  h1 {
    font-size: 2.7rem;
  }

  p {
    font-size: 1.5rem;
  }
}
</style>
