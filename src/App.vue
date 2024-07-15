<template>
  <div class="container my-6 mx-auto">
    <div class="thumbnails gap-3 grid justify-center">
      <ThumbnailCard v-for="thumbnail in thumbnails" :key="thumbnail.id" :thumbnail="thumbnail" />
    </div>
  </div>
</template>

<script>
import ThumbnailCard from './components/ThumbnailCard.vue'

export default {
  name: 'App',
  components: {
    ThumbnailCard
  },
  data() {
    return {
      thumbnails: [
        { id: 1, title: 'nature_1.jpeg', url: 'src/assets/nature_1.jpeg' },
        { id: 2, title: 'nature_2.jpeg', url: 'src/assets/nature_2.jpeg' },
        { id: 3, title: 'nature_3.jpeg', url: 'src/assets/nature_3.jpeg' },
        { id: 4, title: 'nature_4.jpeg', url: 'src/assets/nature_4.jpeg' },
        { id: 5, title: 'nature_5.jpeg', url: 'src/assets/nature_5.jpeg' },
        { id: 6, title: 'nature_6.jpeg', url: 'src/assets/nature_6.jpeg' },
        { id: 7, title: 'nature_7.jpeg', url: 'src/assets/nature_7.jpeg' },
        { id: 8, title: 'nature_8.jpeg', url: 'src/assets/nature_8.jpeg' },
        { id: 9, title: 'nature_9.jpeg', url: 'src/assets/nature_9.jpeg' },
        { id: 10, title: 'nature_10.jpeg', url: 'src/assets/nature_10.jpeg' },
        { id: 11, title: 'nature_11.jpeg', url: 'src/assets/nature_11.jpeg' },
        { id: 12, title: 'nature_12.jpeg', url: 'src/assets/nature_12.jpeg' },
        { id: 13, title: 'nature_13.jpeg', url: 'src/assets/nature_13.jpeg' },
        { id: 14, title: 'nature_14.jpeg', url: 'src/assets/nature_14.jpeg' },
        { id: 15, title: 'nature_15.jpeg', url: 'src/assets/nature_15.jpeg' }
      ]
    }
  }
}
</script>

<style scoped>
.thumbnails {
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
}
</style>
