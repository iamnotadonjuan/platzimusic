<template>
  <li>
    <h2>
      <a v-bind:href="artist.url" target="_blank">
        {{ artist.name}}
      </a>
    </h2>
    <img v-bind:src="artist.image[2]['#text']" v-bind:alt="artist.name">
  </li>
</template>

<script>
export default {
  name: 'artist',
  props: ['artist']
}
</script>

<style scoped>
  li {
    display: block;
    margin: 10px 0;
  }
</style>