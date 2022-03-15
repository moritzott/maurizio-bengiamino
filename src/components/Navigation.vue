<template> 
    <router-link :to="{ name: 'home' }">
        <span>Home</span>
    </router-link>
    <router-link :to="{ name: 'about' }">
        <span>About</span>
    </router-link>
    <router-link :to="{ name: 'news' }" >
        <span>News</span>
    </router-link>
    <router-link :to="{ name: 'contact' }">
        <span>Contact</span>
    </router-link>
    <router-link :to="{ name: 'faq' }">
        <span>FAQ</span>
    </router-link>
</template>

<script>
export default {
    name: 'Navigation'
}
</script>

<style scoped>
    /* nur bei der Desktop-Ansicht */
    nav a {
        margin: 0 1em;
        font-size: 18px;
    }

    /* bei Smartphone und Tablet untereinander! */
    @media only screen and (max-width: 952px) {
        nav a {
            display: block;
            margin: 1em 1em;
            font-size: 18px;
        }
    }

</style>
