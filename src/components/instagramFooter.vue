<template>
    <footer class="footer">
            <p><a target="_blank" href="https://about.facebook.com/meta">Meta</a><a target="_blank" href="https://about.instagram.com/">About</a><a target="_blank" href="https://about.instagram.com/blog">Blog</a><a href="https://about.instagram.com/about-us/careers">Jobs</a><a target="_blank" href="https://help.instagram.com/">Help</a><a target="_blank" href="https://developers.facebook.com/docs/instagram">API</a><a href="https://help.instagram.com/519522125107875/?maybe_redirect_pol=0">Privacy</a>
            <a href="https://help.instagram.com/581066165581870">Impressum/Terms/NetzDG/UrhDaG</a><a href="https://www.instagram.com/directory/profiles/">Top Accounts</a><a href="https://www.instagram.com/directory/hashtags/">Hashtags</a><a href="https://www.instagram.com/explore/locations/">Locations</a></p>
            <p><a href="https://www.instagram.com/topics/dance-and-performance/">Dance</a><a href="https://www.instagram.com/topics/food-and-drink/">Food & Drink</a><a href="https://www.instagram.com/topics/home-and-garden/">Home & Garden</a><a href="https://www.instagram.com/topics/music/">Music</a><a href="https://www.instagram.com/topics/visual-arts/">Visual Arts</a></p>
            <p><button>{{ language }}</button>© 2022 Instagram from Meta</p></footer>
        <div v-if="active">
            Menu
        </div>

</template>

<script>
    export default{
        data() {
            return{
            message: "Barcelona"
        };
  }
    }
</script>

<style scoped>
    a {
    color: #9B8E8E;
    font-weight: bold;
    font-size: 11px;
    font-family: 'Roboto', sans-serif;
    padding: 10px;
    text-decoration: none;
  }
    p {
    color: #9B8E8E;
    font-weight: bold;
    font-size: 11px;
    font-family: 'Roboto', sans-serif;
    padding: 10px;
    }

</style>
