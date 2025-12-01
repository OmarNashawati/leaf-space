<script setup></script>

<template>
  <button class="hero-button">
    <slot>Text Here ..</slot>
  </button>
</template>

<style lang="scss" scoped>
.hero-button {
  border: 1px dashed white;
  border-radius: 0.25rem;
  padding: 12px 24px;
  font-weight: 600;
  background: none;
  color: white;
  cursor: pointer;

  &:hover {
    background-color: white;
    color: var(--accent);
  }
}
</style>
