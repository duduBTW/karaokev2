<template>
  <NuxtLink to="/section">
    <div class="home__body-card">
      <div class="home__body-card-images-container">
        <img v-for="url in stream.images" :key="url" :src="url" class="home__body-card-images" />
      </div>
      <div class="home__body-card-titulo">Stream do dia {{ stream.date }}</div>
    </div>
  </NuxtLink>
</template>

<script>
export default {
  name: 'HomeBodyCard',
  props: {
    stream: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style lang="scss" scoped>
.home__body-card {
  background: var(--color-000);
  height: 200px;
  border-radius: 8px;
  overflow: hidden;
  position: relative;

  background: linear-gradient(
    180deg,
    rgba(0, 0, 0, 0) 0%,
    rgba(0, 0, 0, 0.9) 100%
  );

  .home__body-card-titulo {
    font-weight: 500;
    font-size: 20px;
    line-height: 140%;
    position: absolute;
    bottom: 20px;
    left: 20px;
    right: 20px;
  }

  .home__body-card-images-container {
    width: 100%;
    height: 100%;
    display: flex;

    .home__body-card-images {
      width: 33.333%;
      object-fit: cover;
      z-index: -1;
      border-radius: 10px;
    }
  }
}
</style>