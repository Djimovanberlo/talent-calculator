<template>
  <div id="app">
    <MainContents msg="World of Warcraft Classic+ Talent Calculator"/>
    <ClassesNav msg="ClassesNavigator" />
    <Druid msg="Druid" />
    <!-- Druid will be dynamic for each class(?) with props accordingly. Table and images will be part of component contents-->
  </div>
</template>

<script>
import MainContents from './components/MainContents.vue'
import ClassesNav from './components/ClassesNav.vue'
import Druid from './components/Druid.vue'

export default {
  name: 'App',
  components: {
    MainContents,
    ClassesNav,
    Druid
    // Druid will be state managed per class, via ClassesNav
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
