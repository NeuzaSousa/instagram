<template>
    <div>
        <div id="login">
            <h1 id="title">Instagram</h1>
            <input type="text" call="input" v-model="username" placeholder="Phone number, username, or email" />
            <input type="password" call="input" v-model="password" placeholder="Password" />
            <button @click="login">Log In</button>
            <p><span id="hr">&#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240;</span>&#10240;&#10240;OR&#10240;&#10240;<span id="hr">&#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240; &#10240;</span></p>
            <p><img :src="facebook" id="facebook"><a href="">Login with Facebook</a></p>
            <a href="">Forgot password?</a>
            <p>You can also <a href="https://help.instagram.com/contact/543840232909258">report content you believe is unlawful</a> under the Network Enforcement Act (NetzDG) without logging in.</p>
        </div>
        <div id="sign-up">
            Don't have an account? <a href="">Sign up</a>
        </div>
        <p>Get the app</p>
        <button><a href=""></a>Download on the App Store</button>
        <button @click="toggle"><a href=""></a>Get it on Google Play</button>
        
    </div>
</template>

<script>
    import facebook from "./facebook.png"
    export default{
        data(){
            return{
                username: "",
                password: "",
                facebook: facebook,
                language: "English",
                active: false
            };
        },

        methods:{
            login(username, password) {
                if(username && password) {
                    console.log("Login done");
                } else {
                    console.log("Insert username and password")
                }
            },

            toggle() {
                this.active = !this.active
            }
        }
    };
</script>

<style scoped>
    @import url('https://fonts.googleapis.com/css2?family=Grand+Hotel&display=swap');
    #login {
        background-color: white;
        border: #DBDBDB 1px solid;
        width: 345px; 
    }
    #title {
        font-family: 'Grand Hotel', cursive;
        font-size: 55px;
        text-align: center;
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

    button {
        width: 260px;
        margin-left: 40px;
        padding: 7px;
        margin-top: 10px;
        border: none;
        background-color: #0095F6;
        color: white;
        font-weight: bold; 
        border-radius: 5px;
    }

    ::placeholder {
        color: #9B8E8E;
        font-size: 12px;
    }

    #facebook {
        width: 15px;
    }

    #sign-up {
        background-color: white;
        border: #DBDBDB 1px solid; 
        width: 345px; 
    }

    #hr {
        text-decoration: line-through;
    }

    p {
        text-align: center;
        font-family: 'Roboto', sans-serif;
        font-size: 12px;
        font-weight: bold;
        color: #9B8E8E;
    }

   
</style>
