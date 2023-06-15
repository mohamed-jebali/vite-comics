<script>
import './styles/general.scss'
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'
import AppBonus from './components/AppBonus.vue'
import AppFooterTop from './components/AppFooterTop.vue'


export default{
  components:{
    AppHeader,
    AppContent,
    AppBonus,
    AppFooterTop
  }
}

</script>

<template>
    <AppHeader/>
    <AppContent/>
    <AppBonus/>
    <AppFooterTop/>
</template>

<style lang="scss">

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}


ul{
  list-style-type: none;
}
</style>
