<template>
    <div>
        <ul>
            <li v-for="menutitle in menubar">{{ menutitle.name }} 
                <ul>
                    <li v-for="option in menutitle.options">{{ option }}

                    </li>
                </ul>
            
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
    
</style>