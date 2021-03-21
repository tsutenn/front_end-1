
<template>
  <div id="app"
       v-bind:style="{ backgroundImage: 'url(' + imgSrc + ')', }">
    <navigation></navigation>
    <router-view></router-view>
  </div>
</template>

<script>
import navigation from './components/navigation'
import setUrl from './js/userBackground.js'

export default {
  name: 'App',
  components: {
    "navigation": navigation,
  },
  data(){
    //let url=setUrl();
    return{
      imgSrc: require('./assets/background-image.jpg')
    };
  },
}
</script>

<style>
#app{
  width: 100%;
  height: auto;
  margin: 0 auto;
  background-size: cover;
  background-attachment: fixed;
}
</style>