<script>
import AppHeader from './components/AppHeader.vue';
import HomePage from './pages/HomePage.vue';
import About from './pages/About.vue';
import Skills from './pages/Skills.vue';

export default{
  components:{
    AppHeader,
    HomePage,
    About,
    Skills
  }
}
</script>

<template>
  <div>
    <AppHeader/>
    <HomePage/>
    <hr>
    <About/>
    <hr>
    <Skills/>
  </div>
</template>

<style lang="scss">
  @use './styles/generals.scss' as *;
</style>
