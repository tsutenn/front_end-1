
<template>
  <div id="app">
    <navigation></navigation>
    <router-view></router-view>
  </div>
</template>

<script>
import navigation from './components/navigation'
import Page1 from './components/Page1'
import Page2 from './components/Page2'
export default {
  name: 'App',
  components: {
    "navigation": navigation,
    "page1": Page1,
    "page2": Page2,
  }
}
</script>

<style>
</style>