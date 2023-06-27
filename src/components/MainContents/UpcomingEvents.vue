<template>
    <div class="text-center mb-5">
        <h2>"Academics was committed to my success from the moment I attended an Open House. With the support of caring advisors, professors, and staff i was able to thrive in courses, gain recognition through scholarships, and finish with confidence in my @academics abilities."</h2>
    </div>
    <div class="video-events-container position-relative">
        <div class="video position-relative">
            <button class="position-absolute">play</button>
        </div>
        <div class="events position-absolute d-flex flex-column px-5">

            <div class="text-center bg-danger w-50 m-auto mt-0 mb-5">
                <h3>Upcoming Events</h3>
            </div>
            <div class="d-flex">
                <img class="me-3" src="../../assets/img/svg-1.svg" alt="">

                <p class="mb-0">Princeton offers admission information sessions and student-led tours to campus visitors</p>

                <span></span>
            </div>


        </div>
    </div>
</template>
<script>
export default {
    name:"UpcomingEvents"
}
</script>
<style lang="scss" scoped>
.video-events-container{
    height: 650px;
}
.video{
    width: 60%;
    height: 450px;
    border: 2px solid red;
    background-image: url('../../assets/img/video-bg-3.jpg');
    margin-bottom: 3rem;
    button{
        left: 45%;
        top:50%;
    }
}
.events{
    width: 60%;
    height: 450px;
    border: 2px solid blue;
    top:80px;
    left: 40%;
    background-color: white;
    
    margin-bottom: 3rem;
    img{
        width: 50px;
    }
}    
</style>