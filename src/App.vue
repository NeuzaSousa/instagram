<template>
  <div id="app">
    <div id="main">
      <img id="phone" :src="image"/>
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
  @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@100;300;400&display=swap');

  * {
    margin: 0;
    padding: 0;
  }

  body{
    background-color: #FAFAFA;
  }

  #main {
    display: flex;
    /*grid-template-columns: 1fr 1fr;*/
    margin-top: 50px;
    justify-content: center;
    /*grid-template-rows: 100px 1fr 1fr 1fr 1fr 100px;*/

  }

  #phone {
    width: 400px;
    height: auto;
    padding-right: 30px;
  }





  
</style>
