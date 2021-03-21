<template>
  <div class="Export">
    <h1>Export</h1>
    <searchBar></searchBar>
  </div>
</template>

<script>
import SearchBar from './SearchBar'

export default {
  name: 'Export',
  components: {
    "searchBar": SearchBar,
  },
  data(){
    function t() {
      let d = new Date();
      return d.getHours() + ":" + d.getMinutes() + ":" + d.getSeconds()
    }
    return{
      currently:t(),
    }
  },
  methods: {

  },
};
</script>

<style scoped>
.Export {
  position: static;
  padding: 60px;
  height: 720px;
  width: 1080px;
  background-color: rgba(255, 255, 255, 0.8);
}
h1{
  padding: 0;
  font-size: 100px;
  text-align: center;
  color: rgba(50, 100, 150, 1);
}
</style>