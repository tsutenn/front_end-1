<template>
  <div id="Export">
    <searchBar></searchBar>
    <h1>当前时间：{{currently}}</h1>
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
#Export {
  margin: 0;
  padding: 0;
  height: 920px;
  width: 100%;
}
</style>