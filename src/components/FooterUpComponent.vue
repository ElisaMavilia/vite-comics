<template>
    <footer>
        footer
    </footer>
</template>

<script>
 import {footermenu} from '../data/store.js';
    export default {
        name: 'FooterUpComponent',
        data(){
            return{
                footermenu: [
                    {

                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>

    footer{
        background-image: url('src/assets/img/footer-bg.jpg');
        width: 100%;
        color: white;
    }
</style>