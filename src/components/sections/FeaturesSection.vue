<script setup>
import Button from '../ui/Button.vue'
</script>

<template>
  <div id="services" class="features section">
    <div class="head">
      <h2 class="section-title">Why Choose use?</h2>
      <p class="section-description">
        A wonder serenity has taken prossession of my entire soul, like these sweet mornings of
        spring which i enjoy with my whole heart.
      </p>
    </div>

    <div class="inner-wrap">
      <div class="item">
        <img src="../../assets/icons/Assets-1.png" class="icon" />
        <h3>Help Plantation</h3>
        <p>One morning when Gregor Samsa woke from troubled dreams</p>
        <Button>Read More</Button>
      </div>

      <div class="item">
        <img src="../../assets/icons/Assets-2.png" class="icon" />
        <h3>Tulip Tree</h3>
        <p>One morning when Gregor Samsa woke from troubled dreams</p>
        <Button>Read More</Button>
      </div>

      <div class="item">
        <img src="../../assets/icons/Assets-3.png" class="icon" />
        <h3>Tob Tree</h3>
        <p>One morning when Gregor Samsa woke from troubled dreams</p>
        <Button>Read More</Button>
      </div>

      <div class="item">
        <img src="../../assets/icons/Assets-4.png" class="icon" />
        <h3>Tree Plantation</h3>
        <p>One morning when Gregor Samsa woke from troubled dreams</p>
        <Button>Read More</Button>
      </div>

      <div class="item">
        <img src="../../assets/icons/Assets-5.png" class="icon" />
        <h3>Seaweed Tree</h3>
        <p>One morning when Gregor Samsa woke from troubled dreams</p>
        <Button>Read More</Button>
      </div>

      <div class="item">
        <img src="../../assets/icons/Assets-6.png" class="icon" />
        <h3>Coconut Tree</h3>
        <p>One morning when Gregor Samsa woke from troubled dreams</p>
        <Button>Read More</Button>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.features {
  .head {
    margin-bottom: 4rem;
  }

  .inner-wrap {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1rem;

    @media (max-width: 768px) {
      grid-template-columns: repeat(2, 1fr);
    }

    .item {
      border: 1px dashed gray;
      border-radius: 0.25rem;
      padding: 1rem;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      gap: 1rem;
      flex: 1 1 auto;

      h3 {
        color: var(--accent);
      }

      p {
        color: var(--text-soft);
        font-size: 14px;
        max-width: 280px;
      }

      .icon {
        width: 80px;
        height: 80px;
      }
    }
  }
}
</style>
