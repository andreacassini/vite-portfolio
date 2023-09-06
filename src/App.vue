<script>
import AppHeader from './components/AppHeader.vue';
import HomePage from './pages/HomePage.vue';

export default{
  components:{
    AppHeader,
    HomePage
  }
}
</script>

<template>
  <div>
    <AppHeader/>
    <HomePage/>
  </div>
</template>

<style lang="scss">
  @use './styles/generals.scss' as *;
</style>
