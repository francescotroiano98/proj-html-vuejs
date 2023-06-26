<template>
    <div class="footer-nav">
        <ul class="d-flex justify-content-between">
            <li v-for="footerlink in footerbar">

               <h3>{{ footerlink.name }}</h3> 
                <div v-if="footerlink.name === 'Contact Us'">
                    <p>{{ footerlink.address }}</p>
                    <p>{{ footerlink.phone }}</p>
                    <p>{{ footerlink.email }}</p>
                </div>
                <div class="d-flex flex-column" v-else>
                    <a href="#" class="px-1 mb-2" v-for="link in footerlink.links">{{ link }}</a>
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
a{
    color: black;
}
    
</style>