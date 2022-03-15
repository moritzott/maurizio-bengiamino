<template>
  <div @click="closeMobileNavbar" id="modalNavbar" class="modal-navbar">
        <div class="modal-navbar-content">
            <div class="close-button">
                <span>&times;</span>
            </div>
            
            <slot></slot>
        </div>
    </div>
</template>

<script>
export default {
    methods: {
        closeMobileNavbar() {
            const navbarModal = document.querySelector('.modal-navbar');
            navbarModal.style.display = 'none';
      }
    }
}
</script>

<style scoped>

    .close-button {
        text-align: right;
        margin-top: 1em;
    }
    span {
        /* margin-top: 2em; */
        font-size: 40px;
        /* float: right; */
        cursor: pointer;
        /* display: block; */
        /* margin-bottom: 2em; */
    }
    

</style>