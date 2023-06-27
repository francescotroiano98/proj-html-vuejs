<template>
    <div>
        <ul class="d-flex justify-content-center m-0">
            
            <li class="d-flex flex-column position-relative"  v-for="menutitle in menubar"><a href="#">{{ menutitle.name }}</a>
                <div class="my_option">
                    <a href="#" class="px-1 mb-2" v-for="option in menutitle.options">{{ option }}</a>
                </div>
                  
            </li>
            <button>Sign in</button>  

            
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
        margin-right: 2rem;
    }
a{
    color: black;
    
}    
    .my_option{
        display: none;
        
        
    }
ul li:hover .my_option{

    position: absolute;
    z-index: 1;
    top: 30px;
    width: 80px;
        display: flex;
        flex-direction: column;
        background-color: white;
       
        
    }
</style>