<template>
  <div id="app">
    <div id="main">
      <img :src="image"/>
      <instagram-login />
    </div>
    <instagram-footer />
    
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
  import instagramFooter from "./components/instagramFooter";
  import image from "./image.jpg"
  export default {
    name: 'App',
    components: {
      /* helloWorld,*/
      instagramFooter,
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
  @import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

  #main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    justify-content: space-evenly;
    /*grid-template-rows: 100px 1fr 1fr 1fr 1fr 100px;*/

  }

  body{
    background-color: #FAFAFA;
  }

  
</style>
