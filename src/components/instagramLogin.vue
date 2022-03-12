<template>
    <div>
        <div id="login">
            <h1 id="title">Instagram</h1>
            <input type="text" call="input" v-model="username" placeholder="Phone number, username or email" />
            <input type="password" call="input" v-model="password" placeholder="Password" />
            <button @click="login">Login</button>
            <p>------------ OR ------------</p>
            <img :src="facebook" id="facebook">
            <span>Login with Facebook</span>
            <a href="">Forgot password?</a>
            <p>You can also <a href="https://help.instagram.com/contact/543840232909258">report content you believe is unlawful</a> under the Network Enforcement Act (NetzDG) without logging in.</p>
        </div>
        <div id="sign-up">
            Don't have an account? <a href="">Sign up</a>
        </div>
        <p>Get the app</p>
        <button><a href=""></a>Download on the App Store</button>
        <button @click="toggle"><a href=""></a>Get it on Google Play</button>
        <footer>
            <p><a target="_blank" href="https://about.facebook.com/meta">Meta</a><a target="_blank" href="https://about.instagram.com/">About</a><a target="_blank" href="https://about.instagram.com/blog">Blog</a><a href="https://about.instagram.com/about-us/careers">Jobs</a><a target="_blank" href="https://help.instagram.com/">Help</a><a target="_blank" href="https://developers.facebook.com/docs/instagram">API</a><a href="https://help.instagram.com/519522125107875/?maybe_redirect_pol=0">Privacy</a>
            <a href="https://help.instagram.com/581066165581870">Impressum/Terms/NetzDG/UrhDaG</a><a href="https://www.instagram.com/directory/profiles/">Top Accounts</a><a href="https://www.instagram.com/directory/hashtags/">Hashtags</a><a href="https://www.instagram.com/explore/locations/">Locations</a></p>
            <p><a href="https://www.instagram.com/topics/dance-and-performance/">Dance</a><a href="https://www.instagram.com/topics/food-and-drink/">Food & Drink</a><a href="https://www.instagram.com/topics/home-and-garden/">Home & Garden</a><a href="https://www.instagram.com/topics/music/">Music</a><a href="https://www.instagram.com/topics/visual-arts/">Visual Arts</a></p>
            <p><button>{{ language }}</button>© 2022 Instagram from Meta</p></footer>
        <div v-if="active">
            Menu
        </div>
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
        border: black 1px solid; 
    }
    #title {
        font-family: 'Grand Hotel', cursive;
        margin: auto;
        font-size: 55px;
    }

    .input { 
        background-color: #FAFAFA;
    }

    #facebook {
        width: 15px;
    }

    #sign-up {
        background-color: white;
        border: black 1px solid; 
    }
   
</style>
