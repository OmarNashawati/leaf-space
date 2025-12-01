<script setup></script>

<template>
  <div class="gallery section">
    <div class="head">
      <h2 class="section-title">Paradise Garden</h2>
      <p class="section-description">
        A wonder serenity has taken prossession of my entire soul, like these sweet mornings of
        spring which i enjoy with my whole heart.
      </p>
    </div>

    <div class="gallery-warp">
      <img
        class="image"
        src="@/assets/images/premium_photo-1678648542632-279af47a78ba.jpeg"
        alt=""
      />

      <img
        class="image"
        src="@/assets/images/premium_photo-1664526284238-afa02646da87.jpeg"
        alt=""
      />

      <img class="image" src="@/assets/images/feey-iNVW4MTNPrk-unsplash.jpg" alt="" />

      <img class="image" src="@/assets/images/phil-hearing-p57EUfjtiTo-unsplash.jpg" alt="" />

      <img class="image" src="@/assets/images/feey-CjLi47MSeUg-unsplash.jpg" alt="" />

      <img class="image" src="@/assets/images/annie-spratt-96DJegygiQE-unsplash.jpg" alt="" />

      <img
        class="image"
        src="@/assets/images/premium_photo-1678988086439-33af83922142.jpeg"
        alt=""
      />

      <img
        class="image"
        src="@/assets/images/premium_photo-1682147003117-503b926d51d0.jpeg"
        alt=""
      />
    </div>
  </div>
</template>

<style lang="scss" scoped>
.gallery {
  padding-top: 0;

  .head {
    padding: 2rem 0;
    text-align: center;
  }

  .gallery-warp {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1rem;

    @media (max-width: 768px) {
      grid-template-columns: repeat(2, 1fr);
    }

    .image {
      aspect-ratio: 1/1;
      display: inline-block;
      object-fit: cover;
      width: 100%;
      height: 100%;
    }
  }
}
</style>
