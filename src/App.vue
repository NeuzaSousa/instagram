<template>
  <div id="app">
    <!-- <h1>Hello world</h1> -->
    <hello-world />
    <img :src="image"/>
    <instagram-login />
    
  </div>
</template>

<script>

    /*import image from "./assets/logo.png"
    
    export default {
        data: function () {
            return {
                image: image
            }
        }
    }*/

  //import helloWorld from "./components/HelloWorld";
  import instagramLogin from "./components/instagramLogin";
  import image from "./image.jpg"
  export default {
    name: 'App',
    components: {
      /* helloWorld,*/
      instagramLogin
    },
    data: function(){
      return {
        image: image
      }
    }
  };
</script>

<style>
#app {
  /*display: inline-grid;*/
  /*grid-template-columns: [first] 1fr [img] 1fr [login] 1fr [last] 1fr;*/
  
  /*background-color: black;*/
  /*font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;*/
  
}
body{
  background-color: #FAFAFA;
}
</style>
