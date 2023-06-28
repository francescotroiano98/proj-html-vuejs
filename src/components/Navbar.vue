<template>
    <div>
        <ul class="d-flex justify-content-center align-items-center m-0">
            
            <li class="d-flex flex-column position-relative"  v-for="menutitle in menubar"><a href="#">{{ menutitle.name }}</a>
                <div class="line"></div>
                <div class="my_option">
                    <a href="#" class="px-1 mb-2" v-for="option in menutitle.options">{{ option }}</a>
                </div>
                  
            </li>
            <button class="border-0 py-2 px-3">Sign in</button>  

            
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
        padding-top: 1rem;
        padding-bottom: 1rem;
    }
a{
    color: black;
    
}    
.line{
        display: none;
    }
    .my_option{
        display: none;
        
        
    }
    ul li:hover {
     .line {
        position: absolute;
        bottom: 13px;
        right: 0px;
        height: 2px;
        background-color: #ff5166;
        width: 25px;
    }

        .my_option {
            position: absolute;
            z-index: 1;
            top: 50px;
            left: -3px;
            width: 80px;
            display: flex;
            flex-direction: column;
            background-color: white;
            transition: all 2s ease;
        }
    }
   
    button{
        background-color: white;
        font-weight: 600;
        box-shadow: rgba(0, 0, 0, 0.15) 0px 3px 8px;
    }
    button:hover{
        background-color: #ff5166;
        color: white;
    }
    

    a:hover{
        color: #ff5166;
    }
</style>