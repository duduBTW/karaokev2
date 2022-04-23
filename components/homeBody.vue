<template>
  <div class="home__body-container">
    <home-body-card v-for="stream in streamsList" :key="stream.id" :stream="stream" />
  </div>
</template>

<script>
import homeBodyCard from './homeBodyCard.vue'

export default {
  name: 'HomeBody',
  components: { homeBodyCard },
  data() {
    return {
      streamsList: [
        {
          id: 1,
          date: '12/12/2012',
          images: [
            '/assets/images/97765339_p0_master1200.jpg',
            '/assets/images/97765331_p0_master1200.jpg',
            '/assets/images/97765312_p0_master1200.jpg',
          ],
        },
        {
          id: 2,
          date: '12/12/2012',
          images: [
            '/assets/images/97765339_p0_master1200.jpg',
            '/assets/images/97765331_p0_master1200.jpg',
            '/assets/images/97765312_p0_master1200.jpg',
          ],
        },
        {
          id: 3,
          date: '12/12/2012',
          images: [
            '/assets/images/97765339_p0_master1200.jpg',
            '/assets/images/97765331_p0_master1200.jpg',
            '/assets/images/97765312_p0_master1200.jpg',
          ],
        },
        {
          id: 4,
          date: '12/12/2012',
          images: [
            '/assets/images/97765339_p0_master1200.jpg',
            '/assets/images/97765331_p0_master1200.jpg',
            '/assets/images/97765312_p0_master1200.jpg',
          ],
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.home__body-container {
  grid-column: 5 / -3;
  @media only screen and (max-width: 600px) {
    grid-column: 1 / -1;
  }

  margin-top: 8px;
  display: grid;
  gap: 20px;
  grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
}
</style>