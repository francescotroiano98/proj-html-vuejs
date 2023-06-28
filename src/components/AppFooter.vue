<template>
    <footer>
        <section class="my_container py-5">


            <Newsletter/>

            
            <FooterNavbar :footerbar="footerbar"/>

            


        </section>
    </footer>
    <Copyrights/>
</template>
<script>
import Newsletter from './FooterContents/Newsletter.vue';
import FooterNavbar from './FooterContents/FooterNavbar.vue';
import Copyrights from './FooterContents/Copyrights.vue';
export default {
    name:"AppFooter",
    components:{
    FooterNavbar,
    Newsletter,
    Copyrights
},

    data(){
        return{
            footerbar: [
        {
          name: 'Contact Us',
          address:'900 Wood Street, MI New York 48607',
          phone:'+56 345 678 000-09',
          email:'info@example.com'
        },
        {
          name: 'Explore',
          links: ['Accomodation', 'Arts Academics', 'Central Services', 'Conferencesc and Events', 'Food and Drink']
        },
        {
          name: 'Support Us',
          links: ['Register Activation Key', 'Student Financial Support', 'Student Support', 'Student Union', 'Postgraudate Association']
        },
        {
          name: 'Useful Links',
          links: ['Admission', 'Contact Us', 'FAQs', 'Request information', 'Privacy Notice']
        },
        
      ]
    
        }
        

    },
}
</script>
<style lang="scss">
    footer{
      
        height: 500px;
        background-color: #192735;
    }
</style>