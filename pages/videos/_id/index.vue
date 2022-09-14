<template>
  <div>
    <h2>I want to watch {{video.title}} again. It was an awesome movie</h2>
    <nuxt-link :to="`/videos/${video.id}/watch`">
      <button>Watch</button>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  props: ['video']
}
</script>

<style>

</style>