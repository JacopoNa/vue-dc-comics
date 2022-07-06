<template>
  <div id="app">
      <MainHeader/>

      <MainContent/>

      <MainShop/>

      <MyFooter/>
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue'
import MainContent from './components/MainContent.vue'
import MainShop from './components/MainShop.vue'
import MyFooter from './components/MyFooter.vue'

export default {
  name: 'App',
  components: {
    MainHeader,
    MainContent,
    MainShop,
    MyFooter
  }
}
</script>

<style lang="scss">
  @import './style/common.scss';
  @import './style/variables.scss'
</style>
