<script setup>
import HeartIcon from '@/assets/icons/heart.svg'
</script>

<template>
  <div class="top-services">
    <div class="img-1 service-item">
      <div class="inner-wrap">
        <HeartIcon class="icon" />
        <p>Landing Style</p>
      </div>
    </div>
    <div class="service-item img-2">
      <div class="inner-wrap">
        <HeartIcon class="icon" />
        <p>Irrigation System</p>
      </div>
    </div>
    <div class="service-item img-3">
      <div class="inner-wrap">
        <HeartIcon class="icon" />
        <p>Tree Surgery</p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.top-services {
  display: grid;
  grid-template-columns: repeat(3, 1fr);

  @media (max-width: 768px) {
    grid-template-columns: repeat(1, 1fr);
  }

  .img-1 {
    background: url('@/assets/images/photo-1697269520489-2de855272308.jpeg');
  }
  .img-2 {
    background: url('@/assets/images/premium_photo-1679430139038-c1300dec3d58.jpeg');
  }
  .img-3 {
    background: url('@/assets/images/premium_photo-1723870815044-fd39c225aa89.jpeg');
  }

  .service-item {
    aspect-ratio: 4 / 3;
    background-position: center;
    background-size: cover;

    @media (max-width: 768px) {
      aspect-ratio: 16 / 9;
    }

    &:hover .inner-wrap {
      background: rgba(0, 0, 0, 0);
    }

    .inner-wrap {
      width: 100%;
      height: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: end;
      gap: 1.5rem;
      font-weight: 600;
      padding-bottom: 3rem;
      color: var(--text-on-dark-background);
      background: rgba(0, 0, 0, 0.3);
      cursor: pointer;

      .icon {
        width: 50px;
        height: 50px;
      }

      p {
        font-size: 1.3rem;
      }
    }
  }
}
</style>
