<template>
  <div class="home">
    <Photo 
      image="https://res.cloudinary.com/horlabyc/image/upload/v1594847543/image_vbs2ir.svg"
      title="Jordan Okeke"
      metaData="Pretoria, South Africa"
    />
    <Photo 
      image="https://res.cloudinary.com/horlabyc/image/upload/v1594847543/image_vbs2ir.svg"
      title="Jordan Okeke"
      metaData="Pretoria, South Africa"
    />
    <Photo 
      image="https://res.cloudinary.com/horlabyc/image/upload/v1594847543/image_vbs2ir.svg"
      title="Jordan Okeke"
      metaData="Pretoria, South Africa"
    />
    <Photo 
      image="https://res.cloudinary.com/horlabyc/image/upload/v1594847543/image_vbs2ir.svg"
      title="Jordan Okeke"
      metaData="Pretoria, South Africa"
    />
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

<style lang="scss" scoped>
  .home {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(250px,1fr));
  }
</style>