<script>
import './styles/general.scss'
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppBonus from './components/AppBonus.vue'
import AppFooterTop from './components/AppFooterTop.vue'
import AppFooterBottom from './components/AppFooterBottom.vue'


export default{
  components:{
    AppHeader,
    AppContent,
    AppBonus,
    AppFooterTop,
    AppFooterBottom
  }
}

</script>

<template>
    <AppHeader/>
    <AppContent/>
    <AppBonus/>
    <AppFooterTop/>
    <AppFooterBottom/>
</template>

<style lang="scss">

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{
  font-family: 'Fira Sans', sans-serif;
}

ul{
  list-style-type: none;
}
</style>
