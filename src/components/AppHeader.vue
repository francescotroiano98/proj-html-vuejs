<template>
    <header>
        <Navbar :menubar="menubar"/>
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

    header{
        height: 200px;
        background-color: red;
    }
</style>