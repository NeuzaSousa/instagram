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
    margin-top: 50px;
    justify-content: center;
  }

  #phone {
    width: 400px;
    height: auto;
    padding-right: 30px;
  }

  @media screen and (max-width: 875px) {
    #phone {
      display: none;
    }
  }

  @media screen and (max-width: 450px) {
    #login {
      width: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      margin-top: none;
      border: none;
      background-color: #FAFAFA;
    }

    #sign-up {
      display: flex;
      justify-content: center;
      width: 100%;
      border: none;
      background-color: #FAFAFA;
    }
  }

  





  
</style>
