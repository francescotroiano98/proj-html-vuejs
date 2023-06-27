<template>
    <section class="my_container">
        <Description/>
        <RecentCourses/>
        <UpcomingEvents/>
        <Latest/>
        
    </section>
</template>
<script>
import Description from './MainContents/Description.vue';
import RecentCourses from './MainContents/RecentCourses.vue'
import UpcomingEvents from './MainContents/UpcomingEvents.vue'
import Latest from './MainContents/Latest.vue';
export default {
    name:"AppMain",
    components:{
        Description,
        RecentCourses,
        UpcomingEvents,
        Latest
    }
}
</script>
<style lang="scss">
    
</style>