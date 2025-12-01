<script setup></script>

<template>
  <button>
    <slot>Text Here..</slot>
  </button>
</template>

<style lang="scss" scoped>
button {
  background: var(--accent);
  border: none;
  outline: none;
  padding: 8px 16px;
  color: white;
  border-radius: 0.25rem;
  font-size: 12px;
  cursor: pointer;

  &:hover {
    background: var(--accent-soft);
  }
}
</style>
