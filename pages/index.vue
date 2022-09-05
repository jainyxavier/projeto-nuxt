<template>
    <div>
        <TheHeader/>
        <section class="section-banner">
            <div class="container">
                <div class="title-section">
                    <h1>Managing your crypto portfolio has never been easier</h1>

                    <p>End-to-end payments and financial management in a single solution. Meet the right platform to help realize.</p>
                </div>

                <div class="box-btn">
                    <a href="#">Get Started</a>

                    <div class="btn-play">
                        <div></div><a href="#">See How It Works</a>
                    </div>
                </div>

                <div class="portfolio">
                    <nuxt-img src="img/banner-portfolio.png" />
                </div>
            </div>
        </section>

        <section class="section-sponsorship">
            <div class="container">
                <div class="title-sponsorship">
                    <h2>Over 32k+ software  businesses growing with AR Shakir.</h2>
                </div>

                <div class="content-brands">
                    <BrandsImage url="img/brands/open.svg" />
                    <BrandsImage url="img/brands/oracle.svg" />
                    <BrandsImage url="img/brands/morpheus.svg" />
                    <BrandsImage url="img/brands/samsung.svg" />
                    <BrandsImage url="img/brands/monday.svg" />
                    <BrandsImage url="img/brands/segment.svg" />
                    <BrandsImage url="img/brands/protonet.svg" />
                </div>
            </div>
        </section>
    </div>
</template>

<script>
    import BrandsImage from "~/components/BrandsImage"

    export default {
        name: 'IndexPage',
        data(){
            return{
                url: ''
            }
        },

        components: {
            childComponent: BrandsImage
        }
}
</script>

<style lang="scss">

</style>