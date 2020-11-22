<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <Photo />
  </div>
</template>

<script>
// @ is an alias to /src
import Photo from '../components/shared/photo.vue';

export default {
  name: 'Home',
  components: {
    Photo
  }
}
</script>
