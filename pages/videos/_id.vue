<template>
  <h2>I want to watch {{video.title}} again. It was an awesome movie</h2>
</template>

<script>
export default {
  
/* Data containng the videos */
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

  computed: {
    video() {
      return this.videos.find(v => v.id == this.$route.params.id)
    }
  }
}
</script>

<style>

</style>