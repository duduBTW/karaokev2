<template>
  <div class="section">
    <section-navegation />
    <section-content />
  </div>
</template>

<script>
import SectionContent from '~/components/sectionContent.vue'
import sectionNavegation from '~/components/sectionNavegation.vue'
export default {
  name: 'SectionPage',
  components: { sectionNavegation, SectionContent },
}
</script>

<style lang="scss" scoped>
.section {
  display: grid;
  grid-template-columns: repeat(20, 1fr);
  gap: 20px;

  @media only screen and (max-width: 600px) {
    grid-template-columns: repeat(4, 1fr);
    margin: 0px 20px;
  }
}
</style>
