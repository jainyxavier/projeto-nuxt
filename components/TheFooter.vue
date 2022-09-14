<template>
    <div>
        <footer>
            <div class="container">
                <div class="title-footer">
                    <h2>Join millions of<br> creative people with AR Shakir</h2>

                    <TheBtn 
                    :textBtn="theBtn.textBtn='Join The Waitlist'" 
                    :colorBtn="theBtn.colorBtn='#F9896B'" 
                    :linkBtn="theBtn.linkBtn='#'" />
                </div>
            </div>

            <div class="line"></div>

            <div class="container">
                <div class="info-footer">
                    <div class="about-us">
                        <h4>Ar Shakir</h4>
                        <p>Yet bed any for travelling assistance indulgence unpleasing. Not thoughts all exercise blessing. Indulgence way everything joy alteration boisterous the attachment.</p>
                    </div>

                    <div class="box-services">
                        <ServicesFooter
                        :title="servicesFooter.title='Company'"
                        :items="[servicesFooter.items[0]='About Us', servicesFooter.items[1]='Careers', servicesFooter.items[2]='Blog', servicesFooter.items[3]='Pricing']" />
                    
                        <ServicesFooter
                        :title="servicesFooter.title='Product'"
                        :items="[servicesFooter.items[0]='Invoicing Platform', servicesFooter.items[1]='Accounting Plateform', servicesFooter.items[2]='Create Proposal', servicesFooter.items[3]='Contracts']" />
                    
                        <ServicesFooter
                        :title="servicesFooter.title='Resources'"
                        :items="[servicesFooter.items[0]='Proposal Template', servicesFooter.items[1]='Invoice Template', servicesFooter.items[2]='Tuturoial', servicesFooter.items[3]='How to write a contract']" />
                    </div>
                </div>
            </div>

            <div class="line"></div>

            <div class="container">
                <div class="credits">
                    <p>2022 AR Shakir. All rights reserved. -- Privacy Policy - Terms of Services</p>

                    <span>Supported by Microsoft Startup</span>
                </div>
            </div>
        </footer>
    </div>
</template>

<script>
    import TheBtn from "~/components/TheBtn"
    import ServicesFooter from "~/components/ServicesFooter"

export default {
    name: 'IndexPage',
    data(){
        return{
            theBtn:{
                textBtn: '',
                colorBtn: '',
                linkBtn: ''
            },
            servicesFooter:{
                title: '',
                items: []
            }
        }
    },

    components: {
        childComponent: TheBtn, ServicesFooter
    }
}
</script>