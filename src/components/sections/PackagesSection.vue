<script setup></script>

<template>
  <div id="prices" class="prices-section section">
    <div class="head">
      <h2 class="section-title">Service Packages</h2>
      <p class="section-description">
        One morning when Gregor Samsa woke from troubled dreams. he found himself transformed in his
        bed into a horrible vermin
      </p>
    </div>

    <div class="packages">
      <div class="item">
        <div class="package-info">
          <p class="package-name">Starter Package</p>
          <p class="package-price">
            <span class="unit">$</span><span class="price">34</span><span class="cents">99</span>
          </p>

          <button>Select Plan</button>
        </div>
        <div class="package-details">
          <p><span>✓</span>tree plantation</p>
          <p><span>✓</span> flower garden</p>
          <p><span>✓</span> Tob tree irregation</p>
        </div>
      </div>

      <div class="item">
        <div class="package-info">
          <p class="package-name">Basic Package</p>
          <p class="package-price">
            <span class="unit">$</span><span class="price">49</span><span class="cents">99</span>
          </p>

          <button>Select Plan</button>
        </div>
        <div class="package-details">
          <p><span>✓</span> tree plantation</p>
          <p><span>✓</span> flower garden</p>
          <p><span>✓</span>Tob tree irregation</p>
        </div>
      </div>

      <div class="item">
        <div class="package-info">
          <p class="package-name">Irrigation Package</p>
          <p class="package-price">
            <span class="unit">$</span><span class="price">59</span><span class="cents">99</span>
          </p>

          <button>Select Plan</button>
        </div>
        <div class="package-details">
          <p><span>✓</span> tree plantation</p>
          <p><span>✓</span> flower garden</p>
          <p><span>✓</span>Tob tree irregation</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.prices-section {
  text-align: center;

  .head {
    margin-bottom: 4rem;
  }

  .packages {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 1rem;

    @media (max-width: 768px) {
      flex-direction: column;
    }

    .item {
      display: flex;
      border-radius: 0.25rem;

      @media (max-width: 768px) {
        width: 100%;
      }

      .package-info {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding-bottom: 16px;
        gap: 16px;

        .package-name {
          background: var(--secondary);
          color: var(--primary);
          padding: 16px 16px;
          font-weight: 600;
          font-size: 1rem;

          @media (max-width: 768px) {
            width: 100%;
          }
        }

        .package-price {
          display: flex;
          align-items: start;
          gap: 2px;
          min-height: 100px;
          color: var(--accent);
          font-weight: 900;

          .price {
            font-size: 2.3rem;
            line-height: 1;
          }
        }
        button {
          display: inline-block;
          background: gray;
          padding: 8px 16px;
          color: white;
          border: none;
          font-size: 0.8rem;
          border-radius: 0.25rem;
          cursor: pointer;
        }
      }

      .package-details {
        display: flex;
        flex-direction: column;
        align-items: start;
        justify-content: center;
        flex: 1;
        padding: 0 1rem;
        gap: 10px;

        p {
          color: var(--text-soft);
          font-size: 0.8rem;

          span {
            color: var(--accent);
            font-weight: 600;
            margin-right: 8px;
          }
        }
      }
    }
  }
}
</style>
