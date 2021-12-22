<template>
  <div id="app">
      <div class="app_wrapper">
        <Header />
      <main>
        <DiscCollection />
      </main>
    </div>
    
    
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import Header from "./components/Header.vue";
import DiscCollection from "./components/DiscCollection.vue";


export default {
  name: "App",
  components: {
    Header,
    DiscCollection,
    
  },
};
</script>

<style lang="scss">
@import './style/variables';
@import './style/general';

.app_wrapper{
  width: 100%;
  height: 100vh;
  position: relative;
  background-color: $brand-main-color;
}



</style>
