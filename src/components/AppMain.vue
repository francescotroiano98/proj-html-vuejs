<template>
    <section class="my_container">
        <Description/>
        <RecentCourses/>
        <UpcomingEvents/>
    </section>
</template>
<script>
import Description from './MainContents/Description.vue';
import RecentCourses from './MainContents/RecentCourses.vue'
import UpcomingEvents from './MainContents/UpcomingEvents.vue'
export default {
    name:"AppMain",
    components:{
        Description,
        RecentCourses,
        UpcomingEvents
    }
}
</script>
<style lang="scss">
    
</style>