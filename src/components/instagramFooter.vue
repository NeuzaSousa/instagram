<template>
    <footer class="footer">
            <p><a target="_blank" href="https://about.facebook.com/meta">Meta</a><a target="_blank" href="https://about.instagram.com/">About</a><a target="_blank" href="https://about.instagram.com/blog">Blog</a><a href="https://about.instagram.com/about-us/careers">Jobs</a><a target="_blank" href="https://help.instagram.com/">Help</a><a target="_blank" href="https://developers.facebook.com/docs/instagram">API</a><a href="https://help.instagram.com/519522125107875/?maybe_redirect_pol=0">Privacy</a>
            <a href="https://help.instagram.com/581066165581870">Impressum/Terms/NetzDG/UrhDaG</a><a href="https://www.instagram.com/directory/profiles/">Top Accounts</a><a href="https://www.instagram.com/directory/hashtags/">Hashtags</a><a href="https://www.instagram.com/explore/locations/">Locations</a></p>
            <p><a href="https://www.instagram.com/topics/dance-and-performance/">Dance</a><a href="https://www.instagram.com/topics/food-and-drink/">Food & Drink</a><a href="https://www.instagram.com/topics/home-and-garden/">Home & Garden</a><a href="https://www.instagram.com/topics/music/">Music</a><a href="https://www.instagram.com/topics/visual-arts/">Visual Arts</a></p>
            <p><select name="language" id="language">
                    <option value="afrikaans">Afrikaans</option>
                    <option value="cestina">Cestina</option>
                    <option value="dansk">Dansk</option>
                    <option value="deutsch">Deutsch</option>
                    <option value="english" selected>English</option>
                    <option value="english uk">English (UK)</option>
                    <option value="espanhol espanha">Español (Espanã)</option>
                    <option value="espanhol">Español</option>
                    <option value="suomi">Suomi</option>
                    <option value="francais">Français</option>
                    <option value="bahasa indonesia">Bahasa Indonesia</option>                 
                    <option value="italiano">Italiano</option>                 
                    <option value="bahasa melaio">Bahasa Melaio</option>                 
                    <option value="norsk">Norsk</option>
                    <option value="nederlands">Nederlands</option>
                    <option value="polski">Polski</option>
                    <option value="portugues brasil">Português (Brasil)</option>
                    <option value="portugues portugal">Português (Portugal)</option>
                    <option value="svenska">Svenska</option>
                    <option value="filipino">Filipino</option>
                    <option value="turkce">Türkçe</option>
                    <option value="hrvatski">Hrvatski</option>
                    <option value="magyar">Magyar</option>
                    <option value="slovencina">Slovencina</option>
                    <option value="tieng viet">Tieng Viet</option>
                    <option value="francais canada">Français (Canada)</option>
                    <option value="romana">Romana</option>

                </select> © 2022 Instagram from Meta</p>

    </footer>
</template>

<!-- <script type="text/javascript" src="node_modules/vuejs/dist/vue.min.js"></script>
<script type="text/javascript" src="node_modules/vue-simple-search-dropdown/dist/vue-simple-search-dropdown.min.js"></script>
<script type="text/javascript">
    Vue.use(Dropdown);
</script> -->
<script>
    //import dropdownMenu from './dropdownMenu';
    //import dropdownLanguage from "./dropdownLanguage";
    export default{
        name: "instagramFooter",

    }

</script>

<style scoped>
    a {
        color: #6b6363;
        font-weight: bold;
        font-size: 12px;
        font-family: 'Roboto', sans-serif;
        padding: 10px;
        text-decoration: none;
        font-weight: 300;
    }

    p {
        color: #6b6363;
        font-weight: bold;
        font-size: 12px;
        font-family: 'Roboto', sans-serif;
        padding: 10px;
        text-align: center;
        font-weight: 300;
    }

    footer {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        justify-content: center;
        padding-top: 50px;
        padding-bottom: 50px;
    }

    select#language {
        border:0px;
        outline:0px;
        width: 65px;
        color: #6b6363;
        font-size: 12px;
        margin-right: 15px;
    }

</style>
