<template>
    <div>
        <ul class="d-flex">
            
            <li class="d-flex flex-column"  v-for="menutitle in menubar">{{ menutitle.name }} 
                
                    <a href="#" v-for="option in menutitle.options">{{ option }}</a>
            </li>
            
        </ul>
    </div>
</template>
<script>
export default {
    name:"Navbar",
    props:{
        menubar:Object
    }
}
</script>
<style lang="scss" scoped>
    li{
        list-style: none;
        margin-right: 2rem;
    }
</style>