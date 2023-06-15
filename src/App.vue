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


  // GOOGLE FONTS
  // SANS CAPTION
  @import url('https://fonts.googleapis.com/css2?family=PT+Sans+Caption:wght@400;700&display=swap');

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body{
  font-family: 'PT Sans Caption', sans-serif;
}

ul{
  list-style-type: none;
}

a{
  text-decoration: none;
}
</style>
