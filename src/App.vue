<script>
import AppHeader from './components/AppHeader.vue';
import HomePage from './pages/HomePage.vue';
import About from './pages/About.vue';

export default{
  components:{
    AppHeader,
    HomePage,
    About
  }
}
</script>

<template>
  <div>
    <AppHeader/>
    <HomePage/>
    <hr>
    <About/>
  </div>
</template>

<style lang="scss">
  @use './styles/generals.scss' as *;
</style>
