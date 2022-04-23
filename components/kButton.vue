<template>
  <button class="k-button">
    <slot />
  </button>
</template>

<script>
export default {
  name: 'KButton',
}
</script>

<style lang="scss" soped>
.k-button {
  cursor: pointer;

  background: var(--main);
  border: none;
  outline: none;
  color: var(--color-900);

  font-weight: 500;
  font-size: 20px;
  line-height: 24px;
  text-align: center;
  letter-spacing: 0.02em;

  padding: 12px 40px;
  border-radius: 2222px;

  &:hover {
    background: var(--main-l);
  }
}
</style>