<script setup></script>

<template>
  <div id="reviews" class="review">
    <div class="inner-wrapper">
      <h2>Customers Reviews</h2>

      <div class="item">
        <img class="avatar" src="https://avatar.iran.liara.run/public/3" alt="avatar" />
        <div>
          <p>Its amazing service, i recommended it</p>
          <p>John Doe</p>
        </div>
      </div>

      <div class="angled-div"></div>
      <div class="angled-div-2"></div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.review {
  background: url('@/assets/images/premium_photo-1677756430413-24becbc9964e.jpeg');
  background-size: cover;
  background-position: center;
  height: 380px;
  position: relative;

  .inner-wrapper {
    color: var(--text-on-dark-background);
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-evenly;
    gap: 1rem;
    height: 100%;
    background: rgba(0, 0, 0, 0.3);
  }

  h2 {
    color: rgba($color: var(--text-on-dark-background), $alpha: 0.8);
    font-size: 1.5rem;
  }

  .item {
    background: rgba($color: white, $alpha: 0.8);
    border: 3px dotted var(--accent);
    border-radius: 0.25rem;
    padding: 16px 32px;
    color: var(--text);
    display: flex;
    align-items: center;
    gap: 20px;

    .avatar {
      display: inline-block;
      width: 60px;
    }
  }

  .angled-div {
    background-color: white;
    height: 80px;
    width: 100%;
    position: absolute;
    bottom: 0;
    clip-path: polygon(0 0, 100% 80%, 100% 100%, 0% 100%);
  }

  .angled-div-2 {
    background-color: white;
    height: 80px;
    width: 100%;
    position: absolute;
    bottom: 0;
    clip-path: polygon(0 80%, 100% 0, 100% 100%, 0% 100%);
  }
}
</style>
