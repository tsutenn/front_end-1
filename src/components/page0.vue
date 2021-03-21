<template>
  <div id="page0">
    <Export></Export>
    <h1>备案号?不存在的</h1>
  </div>
</template>

<script>
import Export from "@/components/Export.vue";

export default {
name: "page0",
  components: {
    'Export': Export
  }
}
</script>

<style scoped>
#page0{
  margin: 0;
  height: 100%;
  width: 100%;
}
.Export{
  margin: 80px auto 0 auto;
  min-width: 1080px;
}
h1{
  position: static;
  margin: 200px auto 0 auto;
  width: 300px;
  text-align: center;
}
</style>