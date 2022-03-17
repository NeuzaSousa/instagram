<template>
    <div>
        <div id="login">
            <h1 id="title">Instagram</h1>
            <input type="text" call="input" v-model="username" placeholder="Phone number, username, or email" />
            <input type="password" call="input" v-model="password" placeholder="Password" />
            <button :disabled="(!username.length || password.length<5)" id="loginButton" @click="login">Log In</button> 
            <p id="or"><span id="hr">&#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240;</span>&#10240;&#10240;OR&#10240;&#10240;<span id="hr">&#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240;</span></p>
            <p><img :src="facebook" id="facebookImg"><a id="facebookLogin" href="https://www.instagram.com/fxcal/disclosure/?next=%2F">Log in with Facebook</a></p>
            <a id="forgotPassword" href="https://www.instagram.com/accounts/password/reset/">Forgot password?</a>
            <p id="netzDG">You can also <a href="https://help.instagram.com/contact/543840232909258">report content you believe is unlawful</a> under the Network Enforcement Act (NetzDG) without logging in.</p>
        </div>
        <div id="sign-up">
            <p>Don't have an account? <a href="https://www.instagram.com/accounts/emailsignup/">Sign up</a></p>
        </div>
        <p id="getApp">Get the app.</p>
        <button class="black"><a target="_blank" href="https://apps.apple.com/app/instagram/id389801252?vt=lo"><img :src="apple" class="icon" /><span id="firstLineApple">Download on the</span><br><span id="secondLineApple">App Store</span></a></button>
        <button class="black"><a target="_blank" href="https://play.google.com/store/apps/details?id=com.instagram.android&referrer=utm_source%3Dinstagramweb&utm_campaign=loginPage&ig_mid=7A0CC0B8-4420-4882-A51B-965D4A590A1A&utm_content=lo&utm_medium=badge"><img :src="play" class="icon" /><span id="firstLinePlay">GET IT ON</span><br><span id="secondLinePlay">Google Play</span></a></button>
        
    </div>
</template>

<script>
    import facebook from "./facebook.png"
    import apple from "./apple.jpg"
    import play from "./play.jpg"
    export default{
        data(){
            return{
                username: "",
                password: "",
                facebook: facebook,
                apple: apple,
                play: play,
                active: true,
            };
        },

        methods:{
            login(username, password) {
                if(username !== null && password !== null) {
                    alert("Login done");
                } else {console.log("username:", this.username, "password:", this.password);
                    alert("Sorry, your password was incorrect. Please double-check your password.")
                }
            },

        }
    };
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Grand+Hotel&display=swap');
    #login {
        background-color: white;
        border: #DBDBDB 1px solid;
        width: 345px; 
        margin-bottom: 10px;
    }
    #title {
        font-family: 'Grand Hotel', cursive;
        font-size: 53px;
        text-align: center;
        font-weight: 200;
        padding: 15px 0;
        margin-bottom: 10px;
    }

    input {
        width: 240px;
        background-color: #FAFAFA;
        margin-left: 40px; 
        margin-bottom: 5px;
        padding: 10px;
        border: #DBDBDB solid 1px;
        border-radius: 3px;
    }

    #loginButton {
        width: 260px;
        margin-left: 40px;
        padding: 7px;
        margin-top: 10px;
        border: none;
        color: white;
        font-weight: bold; 
        border-radius: 5px;
        background-color: #0095F6;
    }

    #loginButton:disabled {
        cursor: not-allowed;
        border: none;
        background-color: #B2DFFC;
        color: white;
    }

    ::placeholder {
        color: #9B8E8E;
        font-size: 11px;
    }

    #facebookImg {
        width: 17px;
        padding: 10px;
        position: relative;
        left: 80px;
    }

    #sign-up {
        background-color: white;
        border: #DBDBDB 1px solid; 
        width: 345px;
        color: #632663;
        text-align: center;
        font-family: "Roboto", sans-serif;
        font-size: 13.8px;
        letter-spacing: 0.5px;
        padding: 22px 0;
    }

    #sign-up a{
        text-decoration: none;
        color:#3eb0fc;
        font-weight: bold;
    }

    #hr {
        text-decoration: line-through;
    }

    #or {
        text-align: center;
        font-family: 'Roboto', sans-serif;
        font-size: 12px;
        font-weight: bold;
        color: #9B8E8E;
        padding: 20px 0;
    }

    #facebookLogin {
        color: #3B5998;
        font-size: 12.5px;
        font-family: 'Roboto', sans-serif;
        text-decoration: none;
        position: relative;
        top: -13px;
        left: 80px;
        font-weight: bold;
        letter-spacing: 0.5px;
    }

    #forgotPassword {
        color: rgb(61, 61, 61);
        font-size: 12px;
        font-family: 'Roboto', sans-serif;
        text-decoration: none;
        position: relative;
        left: 130px;
    }

    #netzDG {
        font-family: sans-serif;
        font-weight: 100;
        width: 280px;
        font-size: 12px;
        margin: auto;
        padding: 30px 0 20px 0;
        line-height: 1.5;
        color: #9B8E8E;
        text-align: center;
    }

    #netzDG a {
        text-decoration: none;
        color:black;
    }

    #getApp {
        font-family: "Roboto", sans-serif;
        font-weight: 300;
        font-size: 14px;
        margin: 20px 0 20px 130px;
        letter-spacing: 0.25px;
    }

    .black {
        background-color: black;
        width: 140px;
        padding: 3px 0 3px 0;
        margin: 5px;
        border: none;
        border-radius: 5px;
        text-align: left;
        line-height: none;
        position: relative;
        left: 20px;
    }

    .black a {
        color: white;
        font-family: "Roboto", sans-serif;
        text-decoration: none;
    }

    #firstLineApple {
        font-size: 10px;
        letter-spacing: 0.5px;
        
    }

    #secondLineApple {
        font-size: 18px;
        letter-spacing: 0.5px;
    }

    #firstLinePlay {
        font-size: 9px;
    }

    #secondLinePlay {
        font-size: 16px;
    }

    .icon {
        width: 30px;
        float: left;
        padding-left: 5px;
        padding-right: 5px;
    }

   
</style>
