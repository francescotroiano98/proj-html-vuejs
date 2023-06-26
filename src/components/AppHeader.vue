<template>
    <header class="d-flex align-items-center py-3">
        <section class="my_container d-flex justify-content-between align-items-center">
            <div>
                <img src="../img/logo.png" alt="">
            </div>
            <div class="input-group my_input ms-5">
                <input type="text" class="form-control rounded-0" placeholder="Search..." aria-label="" aria-describedby="basic-addon2">
                <span class="input-group-text rounded-0 bg-white" id="basic-addon2"><i class="fa-solid fa-magnifying-glass" style="color: #a8a8a8;"></i></span>
            </div>
            <Navbar :menubar="menubar"/>
        </section>
        
    </header>
    
</template>
<script>
import Navbar from './Navbar.vue'
export default {
    data(){
        return{
            menubar: [
        {
          name: 'Home',
          options: ['Home 1', 'Home 2', 'Home 3', 'Home 4', 'Home 5', 'Home 6']
        },
        {
          name: 'About',
          options: ['Home 1', 'Home 2', 'Home 3']
        },
        {
          name: 'Academy',
          options: []
        },
        {
          name: 'Courses',
          options: []
        },
        {
          name: 'News',
          options: []
        }
      ]
    
        }
        

    },
    name:"AppHeader",
    components:{
        Navbar
    }
}
</script>
<style lang="scss" scoped>
.my_input{
    width: 20%;
}
img{
  width: 100px;
}    
</style>