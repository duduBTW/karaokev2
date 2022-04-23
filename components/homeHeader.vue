<template>
  <div class="home__header-container">
    <h1 class="home__titulo">Streams</h1>
    <k-button>Nova stream</k-button>
  </div>
</template>

<script>
import KButton from './kButton.vue'

export default {
  name: 'HomeHeader',
  components: {
    KButton,
  },
}
</script>

<style lang="scss" scoped>
.home__header-container {
  grid-column: 5 / -3;
  @media only screen and (max-width: 600px) {
    grid-column: 1 / -1;
  }

  display: flex;
  justify-content: space-between;

  .home__titulo {
    font-weight: 700;
    font-size: 32px;
    line-height: 38px;

    letter-spacing: 0.02em;

    color: var(--color-900);
  }
}
</style>