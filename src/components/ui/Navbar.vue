<script setup>
import { onBeforeMount, onBeforeUnmount, ref } from 'vue'
import Logo from './Logo.vue'

const mobile = ref(false)
const mobileNav = ref(false)

function openMobileNav() {
  mobileNav.value = true
}

function handleClickOutside(event) {
  if (!event.target.classList.contains('menu-button')) {
    mobileNav.value = false
  }
}

onBeforeMount(() => {
  document.addEventListener('click', handleClickOutside)
})

onBeforeUnmount(() => {
  document.removeEventListener('click', handleClickOutside)
})
</script>

<template>
  <header>
    <div class="logo-wrapper">
      <Logo />
    </div>

    <nav :class="{ active: mobileNav, 'mobile-nav': mobile }">
      <a href="#hero">Home</a>
      <a href="#services">Services</a>
      <a href="#reviews">Reviews</a>
      <a href="#prices">Price</a>
      <a href="#contact-us">Contact Us</a>
    </nav>
    <button class="menu-button" @click="openMobileNav()">☰</button>
  </header>
</template>

<style lang="scss" scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  color: var(--text-on-dark-background);
  padding: 1rem;

  .logo-wrapper {
    padding: 0 2rem;
  }

  nav {
    &.active {
      display: flex;
    }

    @media (max-width: 768px) {
      position: fixed;
      background: var(--secondary);
      height: 100vh;
      top: 0;
      right: 0;
      display: none;
      flex-direction: column;
      width: 250px;
    }

    a {
      display: inline-block;
      padding: 8px 24px;
      color: var(--text-on-dark-background);
      transition: all 0.5s ease;
      border-bottom: 1px solid transparent;

      &:hover {
        border-bottom-color: var(--accent);
      }

      @media (max-width: 768px) {
        padding: 12px 24px;
        &:hover {
          background: rgba(255, 255, 255, 0.2);
        }
      }
    }
  }

  .menu-button {
    display: none;
    background: none;
    color: var(--text-on-dark-background);
    border: none;
    font-size: 1.5rem;
    cursor: pointer;

    @media (max-width: 768px) {
      display: block;
    }
  }
}
</style>
