<script setup>
import LocationIcon from '@/assets/icons/location-arrow.svg'
import PhoneIcon from '@/assets/icons/phone.svg'
import MailIcon from '@/assets/icons/mail.svg'
import Logo from '../ui/Logo.vue'
</script>

<template>
  <footer>
    <div class="bottom-section">
      <Logo />
    </div>

    <div class="upper-section">
      <div class="item">
        <LocationIcon class="icon" />
        <p class="title">Location</p>
        <p class="details">United States Fund for UNICEF 125 Maiden Lane, 11th Floor New Work</p>
      </div>

      <div class="item">
        <PhoneIcon class="icon" />
        <p class="title">Contact Us</p>
        <p class="details">
          United States of America Phone:
          <i>706-428-2127</i>
          <i> 706-363-8753 </i>
        </p>
      </div>

      <div class="item">
        <MailIcon class="icon" />
        <p class="title">Mailing Adress</p>
        <p class="details">
          <i> info@leafspace.com </i>
          <i> support@leafspace.com </i>
        </p>
      </div>
    </div>

    <div class="copyright">
      <p>© 2024 Leaf Space All Rights Reserved</p>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
footer {
  background: var(--secondary);
  color: var(--text-on-dark-background);
  padding: 4rem;

  @media (max-width: 768px) {
    padding: 2rem;
  }

  .upper-section {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    padding-bottom: 2rem;

    @media (max-width: 768px) {
      grid-template-columns: repeat(1, 1fr);
      gap: 1rem;
    }

    .item {
      display: flex;
      flex-direction: column;
      align-items: center;
      text-align: center;
      gap: 1rem;
      border: 1px dashed var(--accent);
      padding: 2rem;
      border-radius: 0.25rem;
      width: 100%;

      @media (max-width: 768px) {
        padding: 1rem;
      }

      .icon {
        width: 70px;
        height: 70px;
        color: var(--accent);

        @media (max-width: 768px) {
          width: 40px;
          height: 40px;
        }
      }

      .title {
        font-weight: 600;
        font-size: 1.3rem;

        @media (max-width: 768px) {
          font-size: 1.1rem;
        }
      }

      .details {
        display: flex;
        flex-direction: column;
        gap: 4px;
        font-size: 0.9rem;
        color: var(--text-on-dark-background-soft);

        i {
          font-size: inherit;
          color: inherit;
        }
      }
    }
  }

  .bottom-section {
    padding: 2rem 0;
  }

  .copyright {
    p {
      font-size: small;
      text-align: center;
    }
  }
}
</style>
