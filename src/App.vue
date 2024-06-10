<script>
import AppHeader from './components/AppHeader.vue';
import MainContent from './components/MainContent.vue';
import AppFooter from './components/AppFooter.vue';

export default{
  components: {
    AppHeader,
    MainContent,
    AppFooter,
  },
};
</script>

<template>
<div id="app">
  <AppHeader />
  <MainContent />
  <AppFooter />
</div>


</template>

<style>
* {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
