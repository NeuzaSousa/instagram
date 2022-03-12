<template>
  <div id="app">
    <h1>Hello world</h1>
    <hello-world />
    <instagram-login />
    <img :src="image"/>
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

  import helloWorld from "./components/HelloWorld";
  import instagramLogin from "./components/instagramLogin";
  import image from "./image.jpg"
  export default {
    name: 'App',
    components: {
       helloWorld,
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
  display: grid;
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
