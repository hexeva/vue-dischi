<template>
  <div id="app">
    <Header />
    <main>
      <DiscCollection />
    </main>
    
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

.main-app{
  background-color:$brand-main-color;
  // test
  height: 500px;
}


</style>
