<template>
    <footer>
        <section class="my_container py-5">

            <Newsletter/>

            
            <FooterNavbar :footerbar="footerbar"/>


        </section>
    </footer>
</template>
<script>
import Newsletter from './Newsletter.vue';
import FooterNavbar from './FooterNavbar.vue';
export default {
    name:"AppFooter",
    components:{
        FooterNavbar,
        Newsletter
    },

    data(){
        return{
            footerbar: [
        {
          name: 'Contact Us',
          address:'900 Wood Street, MI',
          phone:'3547853439557',
          email:'gino@gmail.com'
        },
        {
          name: 'Explore',
          links: ['Accomodation', 'Arts Academics', 'Central Services']
        },
        {
          name: 'Support Us',
          links: ['Arts Academics', 'Central Services']
        },
        {
          name: 'Useful Links',
          links: ['Arts Academics', 'Central Services']
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