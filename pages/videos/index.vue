<template>
  <div>
    <h1>Videos</h1>
    <div v-for="video in videos" :key="video.id">
      <h3><nuxt-link :to="`/videos/${video.id}`">{{video.title}}</nuxt-link></h3>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return { 
      videos: [{
        id: 1,
        title: 'The sound of Music'
      }, {
        id: 2,
        title: 'Real Steel'
      }, {
        id: 3,
        title: 'Cars 3'
      }]
    }
  },

}
</script>

<style>

</style>