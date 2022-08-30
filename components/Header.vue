<template>
    <header class="menu-superior">
        <div class="container">
            <h1>Logo</h1>

            <nav class="menu-options">
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">Sobre</a></li>
                    <li><a href="#">Serviços</a></li>
                    <li><a href="#">Galeria</a></li>
                    <li><a href="#">Preços</a></li>
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

<style lang="scss" scoped>

.menu-superior{
    width: 100%;
    background-color:  #022730;

    .container{
        width: calc(100% - 40px);
        max-width: 1240px;
        margin: 0 auto;
        padding: 20px 0;

        display: flex;
        justify-content: space-between;
        align-items: center;
        gap: 10px;

        @media(max-width: 992px){
            flex-direction: column;
            gap: 25px;
        }

        @media(max-width: 480px){
            flex-direction: row;
        }
    }

    h1{
        color: #fff;
        font-size: 2rem;

        position: relative;
        z-index: 2;
    }

    .menu-options{
        width: 100%;
        max-width: 844px;

        ul{
            list-style-type: none;

            display: flex;
            justify-content: space-between;
            gap: 10px;

            li{
                a{
                    color: white;
                    font-size: 1.125rem;
                    text-decoration: none;

                    &:hover{
                        color: #FA8F02;
                    }
                }
            }
        }

        @media(max-width: 480px){
            display: none;
        }
    }

    .menu-hamburguer{
        display: none;
        position: relative;
        z-index: 2;

        @media(max-width: 480px){
            display: flex;
            flex-direction: column;
            gap: 6px;

            div{
                width: 24px;
                height: 3px;
                background-color: #fff;
                transition: all 0.2s ease-in-out;
            }
        }
    }

    .bg-mobile{
        display: none;
    }

    &.active{
        .menu-options{
            display: flex;
            margin-top: 20px;

            position: absolute;
            top: 90px;
            left: 0;
            z-index: 2;
            
            ul{
                flex-direction: column;
                gap: 30px;

                text-align: center;
                margin: 0 auto;
            }
        }

        .menu-hamburguer{
            div{
                transition: all 0.2s ease-in-out;

                &:nth-of-type(1){
                    transform: rotate(45deg);
                }

                &:nth-of-type(2){
                    width: 0;
                    transition: unset;
                }

                &:nth-of-type(3){
                    position: absolute;
                    transform: rotate(135deg);
                }
            }
        }

        .bg-mobile{
            width: 100%;
            height: 100vh;

            display: flex;

            position: absolute;
            left: 0;
            top: 77px;
            z-index: 1;
            
            background-color: #00393D;
        }
    }
}

</style>