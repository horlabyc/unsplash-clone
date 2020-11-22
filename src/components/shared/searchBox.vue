<template>
  <div class="searchBox">
    <svg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-search" width="20" height="20" viewBox="0 0 24 24" stroke-width="1.5" stroke="#9E9E9E" fill="none" stroke-linecap="round" stroke-linejoin="round">
      <path stroke="none" d="M0 0h24v24H0z" fill="none"/>
      <circle cx="10" cy="10" r="7" />
      <line x1="21" y1="21" x2="15" y2="15" />
    </svg>
    <input v-model="searchTerm" type="text" placeholder="Search for photo"/>
    <p>{{ searchTerm }}</p>
  </div>
</template>

<script>
  export default {
    name: 'SearchBox',
    props: {

    },
    data() {
    return {
      searchTerm: ''
    }
  }
  }
</script>

<style lang="scss" scoped>
  .searchBox {
    position: relative;
    svg {
      position: absolute;
      top: 23px;
      left: 34px;
    }
    input {
      background: white;
      outline: none;
      border: none;
      text-decoration: none;
      padding: 1.5rem 2.5rem 1.5rem 4rem;
      border-radius: 10px;
      justify-content: center;
      align-items: center;
      -moz-box-shadow: -2px 7px 18px 8px rgba(187,187,187,0.75);
      box-shadow: -2px 7px 18px -1px rgba(187,187,187,0.43);
      -webkit-box-shadow: -2px 7px 18px -1px rgba(187,187,187,0.43);
      -moz-box-shadow: -2px 7px 18px -1px rgba(187,187,187,0.43);
      font-family: 'Quicksand', sans-serif;
    }
  }
</style>