<template>
    <div class="text-center mb-5 title">
        <h2>"Academics was committed to my success from the moment I attended an Open House. With the support of caring <a href="#"> advisors, professors, and staff</a> i was able to thrive in courses, gain recognition through scholarships, and finish <span>with confidence in my</span> <a>@academics</a> <span>abilities.</span>"</h2>
    </div>
    <div class="video-events-container position-relative">
        <div class="video position-relative">
            <button class="position-absolute rounded-5"><i class="fa-solid fa-play"></i></button>
        </div>
        <div class="events position-absolute d-flex flex-column px-5">

            <div class="text-center upcoming w-50 m-auto mt-0 mb-5">
                <h3>Upcoming Events</h3>
            </div>
            <div class="d-flex">
                <img class="me-3" src="../../assets/img/svg-1.svg" alt="">

                <p class="mb-0">Princeton offers admission information sessions and student-led tours to campus visitors</p>
            </div>
            <div class="ms-3">
                <a class="learn-more ms-5">Learn more <i class="fa-solid fa-chevron-right me-1"></i></a>
            </div>
            <div class="d-flex">
                <img class="me-3" src="../../assets/img/svg-2.svg" alt="">

                <p class="mb-0">Princeton offers admission information sessions and student-led tours to campus visitors</p>
            </div>
            <div class="ms-3 mb-5">
                <a class="learn-more ms-5">Learn more <i class="fa-solid fa-chevron-right me-1"></i></a>
            </div>
            <div class="align-self-center">
                <a class="learn-more">Event Locations <i class="fa-solid fa-chevron-right me-1"></i></a>
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
.title{
    width: 85%;
    margin: 0 auto;
}
h2{
    font-size: 1.5rem;
    line-height: 2.5rem;
}
.title a{
    color: #ff5166;
    
}
.title span{
    font-weight: 600;
}
.video-events-container{
    height: 650px;
}
.video{
    width: 60%;
    height: 450px;
 
    background-image: url('../../assets/img/video-bg-3.jpg');
    margin-bottom: 3rem;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
    button{
        left: 45%;
        top:45%;
        height: 60px;
        width: 60px;
        background-color: transparent;
        border: 2px solid #ff5166;
        color: #ff5166;
    }
}
.events{
    width: 60%;
    height: 450px;
    
    top:80px;
    left: 40%;
    background-color: white;
    
    margin-bottom: 3rem;
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
    .upcoming{
        background-color: #ff5166;
        color: white;
        padding: 0.8rem;
    }
    a{
        color: black;
        font-size: 0.8rem;
    }
    a:hover{
        color: #ff5166;
        font-size: 0.8rem;
    }
    img{
        width: 50px;
    }
p.learn-more{
        font-weight: 700;
        font-size: 0.8rem;
    }
}    
</style>