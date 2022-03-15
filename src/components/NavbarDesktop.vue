<template>
  <nav class="navbar-desktop" >
      <Navigation />
  </nav>
</template>

<script>
import Navigation from '@/components/Navigation.vue'
export default {
    components: {
        Navigation
    }
}
</script>

<style scoped>
    nav {
        float: right;
        margin-right: 3em;
    }

/*     nav * {
        margin: 0 1em;
        font-size: 18px;
    }
 */
</style>