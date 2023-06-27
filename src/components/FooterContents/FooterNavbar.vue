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
                    <p v-for="link in footerlink.links"><a href="#" class="px-1 mb-2" ><i class="fa-solid fa-chevron-right me-1" style="color: #a3b5ca;"></i>{{ link }}</a></p>
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
}
p{
    font-size: small;
    color: #a3b5ca;
    i{
        font-size: 0.7rem;
    }
}
a{
    font-size: small;
    color: #a3b5ca;
}
    
</style>