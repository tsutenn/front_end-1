
<template>
  <div id="app"
       :style="{ backgroundImage: 'url(' + showBackgroundStyle + ')' }">
    <navigation></navigation>
    <router-view></router-view>
  </div>
</template>

<script>
import navigation from './components/navigation'

export default {
  name: 'App',
  components: {
    "navigation": navigation,
  },
  data(){
    return{
      showBackgroundStyle: require("./assets/background-image.jpg")
    };
  }
}
</script>

<style>
</style>