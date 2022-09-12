<template>
    <header class="menu-superior">
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

            <div class="menu-hamburguer" v-on:click="clickHamburguer">
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

    methods: {
        clickHamburguer(){
            console.log('teste')
            var menuSuperior = document.querySelector('.menu-superior')
            var menu = document.querySelector('.menu-hamburguer')

            menu.addEventListener('click', function(){
                menuSuperior.classList.toggle('active')
            })
        }
    }
}
</script>