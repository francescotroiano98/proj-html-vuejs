<template>
    <div class="footer-nav">
        <ul class="d-flex justify-content-between">
            <li v-for="footerlink in footerbar">

               <h4>{{ footerlink.name }}</h4> 
                <div v-if="footerlink.name === 'Contact Us'">
                    <p>{{ footerlink.address }}</p>
                    <p>{{ footerlink.phone }}</p>
                    <p>{{ footerlink.email }}</p>
                </div>
                <div class="d-flex flex-column" v-else>
                    <p v-for="link in footerlink.links"><a href="#" class="px-1 mb-2" ><i class="fa-solid fa-chevron-right me-1"></i>{{ link }}</a></p>
                </div>
            </li>
        </ul>
    </div>
</template>
<script>
export default {
    name:'FooterNavbar',
    props:{
        footerbar:Object
    }
}
</script>
<style lang="scss" scoped>
h4{
    color: white;
    font-size: 1.2rem;
}
p{
    font-size: small;
    color: #a3b5ca;
    font-size: 0.7rem;
    i{
        font-size: 0.7rem;
    }
}
a{
    font-size: 0.7rem;
    color: #a3b5ca;
}
a:hover{
    color: #d74d52;
}
 a:hover  i{
    color: #d74d52;
   
}
</style>