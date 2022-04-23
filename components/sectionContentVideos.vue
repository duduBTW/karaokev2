<template>
  <div class="section__content-videos">
    <section-content-video-card v-for="video in videos" :key="video.id" :video="video" />
  </div>
</template>

<script>
import sectionContentVideoCard from './sectionContentVideoCard.vue'
export default {
  name: 'SectionContentVideos',
  components: { sectionContentVideoCard },
  data() {
    return {
      videos: [
        {
          id: 1,
          title:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do',
          request: 'Pessoa',
          data: '22 minutos',
          thumb: '/assets/images/97765339_p0_master1200.jpg',
        },
        {
          id: 2,
          title:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do',
          request: 'Pessoa',
          data: '22 minutos',
          thumb: '/assets/images/97765331_p0_master1200.jpg',
        },
        {
          id: 3,
          title:
            'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do',
          request: 'Pessoa',
          data: '22 minutos',
          thumb: '/assets/images/97765312_p0_master1200.jpg',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scped>
.section__content-videos {
  display: grid;
  margin-top: 24px;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
}
</style>