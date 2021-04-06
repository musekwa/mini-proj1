<template>
  <div id="app">
    <div class="aside">
      <MainBar />
    </div>
    <div class="main-content">
      <router-view />
    </div>
    <div class="footer">
      <FootBar />
    </div>
  </div>
</template>

<script>
import MainBar from './components/MainBar.vue';
import FootBar from './components/FootBar.vue';

export default {
  name: 'App',
  components: {
    MainBar,
    FootBar,
  }
}
</script>

<style>
  .aside {
    height: 100vh;
    position: fixed;
    top: 0;
    left: 0;
    width: 20%;
  }
  .main-content {
    height: 77vh;
    margin-left: 20%;
    border: 2px solid red;
  }
  .footer {
    height: 20vh;
    width: 80%;
    position: fixed;
    bottom: 0;
    right: 0;
    border: 2px solid black;
  }
</style>
