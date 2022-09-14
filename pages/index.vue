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
                    <BrandsImage :url="brandsImage.url='img/brands/open.svg'" />
                    <BrandsImage :url="brandsImage.url='img/brands/oracle.svg'" />
                    <BrandsImage :url="brandsImage.url='img/brands/morpheus.svg'" />
                    <BrandsImage :url="brandsImage.url='img/brands/samsung.svg'" />
                    <BrandsImage :url="brandsImage.url='img/brands/monday.svg'" />
                    <BrandsImage :url="brandsImage.url='img/brands/segment.svg'" />
                    <BrandsImage :url="brandsImage.url='img/brands/protonet.svg'" />
                </div>
            </div>
        </section>

        <section class="section-resource">
            <div class="container">
                <div class="resource-img">
                    <nuxt-img src="img/img-mulher.png"/>
                </div>

                <div class="resource-info">
                    <span>Our feature</span>
                    <h2>All of your portfolios are linked to your AR Shakir account</h2>
                    <p>Why kept very ever home mrs. Considered sympathize ten uncommonly occasional assistance sufficient not. Letter of on become he tended active enable to.</p>

                    <TheBtn 
                    :textBtn="theBtn.textBtn='Get Started'" 
                    :colorBtn="theBtn.colorBtn='#3734A9'" 
                    :linkBtn="theBtn.linkBtn='#'" />
                </div>

            </div>
        </section>

        <section class="section-payment">
            <div class="container">
                <div class="payment-info">
                    <span>Our feature</span>
                    <h2>All payments can be managed from one account</h2>
                    <p>Why kept very ever home mrs. Considered sympathize ten uncommonly occasional assistance sufficient not. Letter of on become he tended active enable to.</p>

                    <TheBtn 
                    :textBtn="theBtn.textBtn='Get Started'" 
                    :colorBtn="theBtn.colorBtn='#3734A9'" 
                    :linkBtn="theBtn.linkBtn='#'" />
                </div>

                <div class="payment-img">
                    <nuxt-img src="img/payment.png"/>
                </div>
            </div>
        </section>

        <section class="section-video">
            <div class="container">
                <div class="title-info">
                    <h2>Yet preference connection unpleasant yet melancholy but end appearance</h2>

                    <TheBtn 
                    :textBtn="theBtn.textBtn='Get Started'" 
                    :colorBtn="theBtn.colorBtn='#FF7F5C'" 
                    :linkBtn="theBtn.linkBtn='#'" />
                </div>

                <div class="content-items">
                    <div class="box-items">
                        <div class="items">
                            <div class="number">1</div>

                            <div class="info-items">
                                <h3>First Working Process</h3>
                                <p>Blessing it ladyship on sensible judgment settling outweigh.</p>
                            </div>
                        </div>

                        <div class="items">
                            <div class="number">2</div>

                            <div class="info-items">
                                <h3>Dedicated Team</h3>
                                <p>Warmly little before cousin sussex entire men set.</p>
                            </div>
                        </div>

                        <div class="items">
                            <div class="number">3</div>

                            <div class="info-items">
                                <h3>24/7 Hours Support</h3>
                                <p>And excellence partiality estimating terminated day everything.</p>
                            </div>
                        </div>
                    </div>

                    <div class="img-video">
                        <nuxt-img src="img/section-video.png"/>
                    </div>
                </div>
            </div>
        </section>

        <section class="section-information">
            <div class="container">
                <div class="information">
                    <div class="title-information">
                        <h2>Germany-based & GDPR Compliant</h2>
                    </div>

                    <div class="box-info">
                        <div class="box-information">
                            <div class="img-information">
                                <nuxt-img src="img/data.svg"/>
                            </div>
                            <p>Data does not<br> leave our servers</p>
                        </div>
                        <div class="box-information">
                            <div class="img-information">
                                <nuxt-img src="img/infrastructure.svg"/>
                            </div>
                            <p>Own<br> infrastructure</p>
                        </div>
                        <div class="box-information">
                            <div class="img-information">
                                <nuxt-img src="img/most.svg"/>
                            </div>
                            <p>Most renowed<br> data centers</p>
                        </div>
                    </div>
                </div>

                <div class="box-cards-information">
                    <div class="card">
                        <h2>Outward clothes promise at gravity.</h2>
                        
                        <p>End-to-end payments and financial management in a single solution. Meet the right platform to help realize.</p>

                        <TheBtn 
                        :textBtn="theBtn.textBtn='Get Started'" 
                        :colorBtn="theBtn.colorBtn='#3734A9'" 
                        :linkBtn="theBtn.linkBtn='#'" />
                    </div>
                    <div class="card">
                        <h2>Sufficient particular impossible.</h2>
                        
                        <p>End-to-end payments and financial management in a single solution. Meet the right platform to help realize.</p>

                        <TheBtn 
                        :textBtn="theBtn.textBtn='Get Started'" 
                        :colorBtn="theBtn.colorBtn='#3734A9'" 
                        :linkBtn="theBtn.linkBtn='#'" />
                    </div>
                </div>
            </div>
        </section>

        <section class="section-blog">
            <div class="container">
                <div class="title-blog">
                    <h2>Recent Blogs</h2>
                </div>

                <div class="card-destaque">
                    <div class="card-content">
                        <span>Best Practices</span>
                        <h3>In design active temper be uneasy. Thirty for remove plenty regard.</h3>
                        <a href="#">Read More <div></div></a>
                    </div>
                    <div class="card-img">
                        <nuxt-img src="img/blog/card-destaque.png"/>
                    </div>
                </div>

                <div class="box-cards-blog">
                    <BoxCards 
                    :title="boxCards.title='Best Practices'"
                    :description="boxCards.description='Partiality on or continuing particular principles as.'"
                    :image="boxCards.image='img/blog/card-one.png'"
                    />

                    <BoxCards 
                    :title="boxCards.title='Best Practices'"
                    :description="boxCards.description='Village did removed enjoyed explain'"
                    :image="boxCards.image='img/blog/card-two.png'"
                    />

                    <BoxCards 
                    :title="boxCards.title='Best Practices'"
                    :description="boxCards.description='Wise busy past both park when an ye no. Nay likely her length.'"
                    :image="boxCards.image='img/blog/card-three.png'"
                    />
                </div>
            </div>
        </section>

        <TheFooter/>
    </div>
</template>

<script>
    import BrandsImage from "~/components/BrandsImage"
    import TheBtn from "~/components/TheBtn"
    import BoxCards from "~/components/BoxCards"

    export default {
        name: 'IndexPage',
        data(){
            return{
                brandsImage:{
                    url: ''
                },
                theBtn:{
                    textBtn: '',
                    colorBtn: '',
                    linkBtn: ''
                },
                boxCards:{
                    title: '',
                    description: '',
                    image: ''
                }
            }
        },

        components: {
            childComponent: BrandsImage, TheBtn, BoxCards
        }
    }
</script>