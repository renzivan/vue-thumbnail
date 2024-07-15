<template>
  <div class="thumbnail rounded-md overflow-hidden border-gray-300 relative h-[400px]">
    <img
      :src="thumbnail.url"
      :alt="thumbnail.title"
      :title="thumbnail.title"
      class="w-full h-full object-cover transition duration-500 ease-in-out"
    />
    <div
      class="download flex justify-center items-center inset-0 opacity-0 absolute transition duration-500 ease-in-out"
    >
      <a
        class="bg-gray-700 text-white rounded-md px-4 py-2"
        :href="thumbnail.url"
        :download="thumbnail.title"
        >DOWNLOAD</a
      >
    </div>
  </div>
</template>

<script>
export default {
  name: 'ThumbnailCard',
  props: {
    thumbnail: Object
  }
}
</script>

<style lang="scss" scoped>
.thumbnail:hover {
  img {
    opacity: 0.3;
  }

  .download {
    opacity: 1;
  }
}
</style>
