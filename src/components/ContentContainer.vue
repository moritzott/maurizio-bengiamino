<template>
<div class="content-of-page">
    <Banner />
    <router-view/>
</div>
  
</template>

<script>
import Banner from './Banner.vue'

export default {
    components: {
        Banner
    }
}
</script>

<style>

</style>