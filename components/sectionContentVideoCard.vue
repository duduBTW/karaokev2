<template>
  <div class="section__content-video-card">
    <img :src="video.thumb" alt="">
    <h3>
      {{video.title}}
    </h3>
    <h4>
      Pedido por {{video.request}} - ha {{video.data}}
    </h4>
  </div>
</template>

<script>
export default {
  name: 'SectionContentVideoCard',
  props: {
    video: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style lang="scss" scoped>
.section__content-video-card {
  box-sizing: border-box;
  position: relative;
  height: 200px;
  border-radius: 8px;
  background: linear-gradient(
    180deg,
    rgba(0, 0, 0, 0) 0%,
    rgba(0, 0, 0, 0.9) 100%
  );
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  gap: 6px;
  padding: 16px;

  h3 {
    color: rgba(255, 255, 255, 0.92);
    margin: 0px;
    padding: 0px;
    font-size: 16px;
    font-weight: 500;
    line-height: 140%;
  }

  h4 {
    margin: 0px;
    padding: 0px;
    font-weight: 400;
    font-size: 12px;
    line-height: 140%;
  }

  img {
    position: absolute;
    object-fit: cover;
    object-position: 50% 20%;
    inset: 0;
    width: 100%;
    height: 100%;
    border-radius: 10px;
    z-index: -1;
  }
}
</style>