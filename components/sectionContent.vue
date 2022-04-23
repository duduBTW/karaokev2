<template>
  <div class="section__navegation">
    <h1>Stream 12/12/2012</h1>
    <section-content-videos />
  </div>
</template>

<script>
import sectionContentVideos from './sectionContentVideos.vue'
export default {
  name: 'SectionContent',
  components: { sectionContentVideos },
}
</script>

<style lang="scss" scoped>
.section__navegation {
  grid-column: 8 / -4;
  margin-top: 60px;

  h1 {
    padding-top: 16px;
    font-size: 20px;
    line-height: 24px;

    letter-spacing: 0.02em;
  }
}
</style>