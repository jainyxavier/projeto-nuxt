<template>
    <section class="section-banner">
        <div class="container">
            <div class="title-section">
                <h2>Managing your crypto portfolio has never been easier</h2>

                <p>End-to-end payments and financial management in a single solution. Meet the right platform to help realize.</p>
            </div>

            <div class="box-btn">
                <a href="#">Get Started</a>

                <div class="btn-play">
                    <div></div><a href="#">See How It Works</a>
                </div>
            </div>
            
            <!-- <div class="banner">
                <nuxt-img src="img/chef-mulher.png" />
            </div> -->
        </div>
    </section>
</template>

<style lang="scss" scoped>
    .section-banner{
        width: 100%;
        position: relative;

        padding: 70px;

        background: rgb(68, 81, 196);
        background: radial-gradient(circle, rgba(68,81,196,1) 0%, rgba(68,81,196,1) 100%);

        &::after, &::before{
            content: '';
            width: 100px;
            height: 500px;
            border-radius: 50%;

            position: absolute;
            filter: blur(30px);
            background: rgb(61, 58, 224);
        }

        &::after{
            top: 0;
            right: -5%;
        }

        &::before{
            top: 0;
            left: -5%;
        }

        .container{
            width: calc(100% - 40px);
            max-width: 920px;
            margin: 0 auto;
        }

        .title-section{
            padding-bottom: 56px;
            text-align: center;

            h2{
                font-size: 3.75rem;
                font-weight: 700;
                color: #fff;
                margin-bottom: 32px;
            }

            p{
                font-size: 1.25rem;
                font-weight: 500;
                color: #fff;
            }
        }

        .box-btn{
            width: 100%;
            max-width: 420px;
            margin: 0 auto;

            display: flex;
            justify-content: space-between;

            a{
                background-color: #dd532d;
                border-radius: 47px;
                padding: 15px 38px;
                
                text-decoration: unset;
                font-size: 1rem;
                color: #fff;

                display: flex;
                align-items: center;
            }

            .btn-play{
                display: flex;
                align-items: center;
                gap: 10px;

                div{
                    width: 60px;
                    height: 60px;

                    border-radius: 47px;
                    background: #22D497;

                    position: relative;

                    &::after{
                        content: '';

                        position: absolute;
                        bottom: 18px;
                        left: 22px;

                        width: 25px;
                        height: 25px;

                        background-color: white;
                        clip-path: polygon(0 0, 0 100%, 100% 50%);
                    }
                }

                a{
                    background: unset;
                    padding: 0;
                }
            }
        }

        // .banner{
        //     img{
        //         width: 100%;
        //         height: 100%;
        //     }
        // }
    }
</style>