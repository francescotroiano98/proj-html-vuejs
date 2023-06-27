<template>
    <section class="my_container">
        <Description/>
        <RecentCourses/>
    </section>
</template>
<script>
import Description from './MainContents/Description.vue';
import RecentCourses from './MainContents/RecentCourses.vue'
export default {
    name:"AppMain",
    components:{
        Description,
        RecentCourses
    }
}
</script>
<style lang="scss">
    
</style>