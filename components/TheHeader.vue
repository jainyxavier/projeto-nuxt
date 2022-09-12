<template>
    <header :class="{active: openMenu}" class="menu-superior">
        <div class="container">
            <div class="title-menu">
                <nuxt-link to="/">AR SHAKIR</nuxt-link>
            </div>

            <nav class="menu-options">
                <ul>
                    <li><a href="#">Product</a></li>
                    <li><a href="#">Template</a></li>
                    <li><a href="#">Blog</a></li>
                    <li><a href="#">Sign In</a></li>
                    <li><a href="#">Start Free</a></li>
                </ul>
            </nav>

            <div class="menu-hamburguer" v-on:click="openHamburguer">
                <div></div>
                <div></div>
                <div></div>
            </div>

            <div class="bg-mobile"></div>
        </div>
    </header>
</template>

<script>
export default {
    name: "Header", 
    data(){
        return{
            openMenu: false
        }
    },

    methods: {
        openHamburguer(){            
            if(this.openMenu == false){
                this.openMenu = true
            } else{
                this.openMenu = false
            }
        }
    }
}
</script>