<script>
import AppHeader from './components/AppHeader.vue';
import HomePage from './pages/HomePage.vue';
import About from './pages/About.vue';
import Skills from './pages/Skills.vue';
import Projects from './pages/Projects.vue';
import Contacts from './pages/Contacts.vue';

export default{
  components:{
    AppHeader,
    HomePage,
    About,
    Skills,
    Projects,
    Contacts
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
    <hr>
    <Projects/>
    <Contacts/>
  </div>
</template>

<style lang="scss">
  @use './styles/generals.scss' as *;
</style>
