<template>
  <div id="app">
    <div id="nav">
      <Navigation/>  
    </div>
    <router-view/>
  </div>
</template>

<script>
import Navigation from '@/components/layaout/Navigation'
export default {
  components:{
    Navigation
  }
}
</script>

<style lang="scss">
  @import './scss/app.scss';
</style>