<template>
  <div class="container my-6 mx-auto">
    <div class="thumbnails gap-3 grid justify-center">
      <ThumbnailCard v-for="thumbnail in thumbnails" :key="thumbnail.id" :thumbnail="thumbnail" />
    </div>
  </div>
</template>

<script>
import ThumbnailCard from './components/ThumbnailCard.vue'
import nature_1 from '@/assets/nature_1.jpeg'
import nature_2 from '@/assets/nature_2.jpeg'
import nature_3 from '@/assets/nature_3.jpeg'
import nature_4 from '@/assets/nature_4.jpeg'
import nature_5 from '@/assets/nature_5.jpeg'
import nature_6 from '@/assets/nature_6.jpeg'
import nature_7 from '@/assets/nature_7.jpeg'
import nature_8 from '@/assets/nature_8.jpeg'
import nature_9 from '@/assets/nature_9.jpeg'
import nature_10 from '@/assets/nature_10.jpeg'
import nature_11 from '@/assets/nature_11.jpeg'
import nature_12 from '@/assets/nature_12.jpeg'
import nature_13 from '@/assets/nature_13.jpeg'
import nature_14 from '@/assets/nature_14.jpeg'
import nature_15 from '@/assets/nature_15.jpeg'

export default {
  name: 'App',
  components: {
    ThumbnailCard
  },
  data() {
    return {
      thumbnails: [
        { id: 1, title: 'nature_1.jpeg', url: nature_1 },
        { id: 2, title: 'nature_2.jpeg', url: nature_2 },
        { id: 3, title: 'nature_3.jpeg', url: nature_3 },
        { id: 4, title: 'nature_4.jpeg', url: nature_4 },
        { id: 5, title: 'nature_5.jpeg', url: nature_5 },
        { id: 6, title: 'nature_6.jpeg', url: nature_6 },
        { id: 7, title: 'nature_7.jpeg', url: nature_7 },
        { id: 8, title: 'nature_8.jpeg', url: nature_8 },
        { id: 9, title: 'nature_9.jpeg', url: nature_9 },
        { id: 10, title: 'nature_10.jpeg', url: nature_10 },
        { id: 11, title: 'nature_11.jpeg', url: nature_11 },
        { id: 12, title: 'nature_12.jpeg', url: nature_12 },
        { id: 13, title: 'nature_13.jpeg', url: nature_13 },
        { id: 14, title: 'nature_14.jpeg', url: nature_14 },
        { id: 15, title: 'nature_15.jpeg', url: nature_15 }
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
