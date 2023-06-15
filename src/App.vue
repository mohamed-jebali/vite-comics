<script>
import './styles/general.scss'
import AppHeader from './components/AppHeader.vue'
import AppContent from './components/AppContent.vue'


export default{
  components:{
    AppHeader,
    AppContent
  }
}

</script>

<template>
  <AppHeader/>
  <AppContent/>
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
