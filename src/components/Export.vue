<template>
  <div id="page">
    <searchBar></searchBar>
    <h1>我是主页</h1>
  </div>
</template>

<script>
import SearchBar from './SearchBar'
export default {
  name: 'Export',
  components: {
    "searchBar": SearchBar
  }
}
</script>

<style scoped>
#page {
  margin: 0;
  padding: 0;
  background: pink;
  height: 600px;
  width: 100%;
}
</style>