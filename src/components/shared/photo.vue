<template>
  <div class="image__wrapper" v-bind:style="{ backgroundImage: 'url(' + image + ')'}">
    <div class="data">
      <p id="title">{{ title }}</p>
      <p id="meta">{{ metaData }}</p>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'Photo',
    props: {
      image: String,
      title: String,
      metaData: String
    }
  }
</script>

<style lang="scss" scoped>
  .image__wrapper {
    background-size: cover;
    border-radius: 5px;
    width: 10rem;
    height: 15rem;
    display: flex;
    background-repeat: no-repeat;
    background-position: 50%;
    .data {
      display: flex;
      flex-direction: column;
      background-color: #00000052;
      width: -webkit-fill-available;
      padding: 1.3rem 0.7rem;
      color: white;
      justify-content: flex-end;
      align-items: flex-start;
      #title {
        font-weight: bold;
        font-size: 0.9rem;
      }
      #meta {
        font-size: 0.8rem;
        font-weight: 500;
      }
    }
  }
</style>