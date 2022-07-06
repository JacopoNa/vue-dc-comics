<template>
  <div id="app">
      <MainHeader/>

      <MainContent/>

      <MainShop/>
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue'
import MainContent from './components/MainContent.vue'
import MainShop from './components/MainShop.vue'

export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    MainShop
  }
}
</script>

<style lang="scss">
  @import './style/common.scss';
  @import './style/variables.scss'
</style>
