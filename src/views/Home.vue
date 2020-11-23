<template>
  <div class="home">
    <SearchBox />
  </div>
</template>

<script>
// @ is an alias to /src
import Photo from '../components/shared/photo.vue';
import SearchBox from '../components/shared/searchBox.vue';

export default {
  name: 'Home',
  components: {
    Photo,
    SearchBox
  }
}
</script>

<style lang="scss" scoped>
  .home {
    /* display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px,1fr)); */
  }
</style>