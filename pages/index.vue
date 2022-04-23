<template>
  <div class="home">
    <home-header />
    <home-body />
  </div>
</template>

<script>
import HomeBody from '~/components/homeBody.vue'
import homeHeader from '~/components/homeHeader.vue'

export default {
  name: 'IndexPage',
  components: { homeHeader, HomeBody },
}
</script>


<style lang="scss" scoped>
.home {
  display: grid;
  grid-template-columns: repeat(20, 1fr);
  gap: 20px;
  padding-top: 60px;

  @media only screen and (max-width: 600px) {
    grid-template-columns: repeat(4, 1fr);
    margin: 0px 20px;
  }
}
</style>
