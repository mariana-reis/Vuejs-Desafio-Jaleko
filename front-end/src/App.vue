<template>

  <div id="app">
       <Video/>
       <Header/>
        <img src="./assets/icon.png">
        <img src="./assets/icon.png">
        <img src="./assets/icon.png">
  </div>

</template>

<script>
import Header from './components/Header'
import Video from "./components/Video";


export default {
  name: "App",
  components: {
     Header,
     Video
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: whitesmoke;
}
</style>
