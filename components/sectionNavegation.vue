<template>
  <div class="section__navegation">
    <div class="section_navegation_item">Próximas</div>
    <div class="section_navegation_item">Set List</div>
  </div>
</template>

<script>
export default {
  name: 'SectionNavegation',
}
</script>

<style lang="scss" scoped>
.section__navegation {
  box-sizing: border-box;
  min-height: 100vh;
  border-right: 1px solid rgba(255, 255, 255, 0.1);
  margin-right: 20px;
  grid-column: 4 / 8;
  padding-top: 60px;

  .section_navegation_item {
    cursor: pointer;

    padding: 12px;
    font-size: 20px;
    line-height: 24px;
  }
}
</style>