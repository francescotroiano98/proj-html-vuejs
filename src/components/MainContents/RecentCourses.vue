<template>
    <div class="title text-center mb-5">
        <h2 class="mb-3">Recent Courses</h2>
        <p>Whether you're considering a foundation course or an undergraduate degree master's or a PhD, academics is a place where students thrive.</p>
    </div>
    <div class="d-flex flex-wrap justify-content-between">
           
           <div class="my_card mb-3">

                <div class="mb-3">
                    <img src="../../assets/img/12786.jpg" alt="">
                </div>
                
                <div class="text-start px-2">
                    <span class="mb-3">$150.00</span>   
                    <h3 class="mb-3">Google Analytics Certification: Earn More</h3>
                    <p class="mb-3">Become Google Analytics Certified to Land a Job, Get Promoted, or Start a New Career...</p>
                    <span class="author">Course by:Tophive</span>
                </div>

            </div>
            
            <div class="my_card mb-3">

                <div class="mb-3">
                    <img src="../../assets/img/7787.jpg" alt="">
                </div>

                <div class="text-start px-2">
                    <span class="mb-3">$55.00</span>   
                    <h3 class="mb-3">Digital Marketing Masterclass - 23 Courses</h3>
                    <p class="mb-3">Grow Your Business with Digital Marketing: Social Media Marketing, Facebook, Content, YouTube, Email Marketing, Websites</p>
                    <span class="author">Course by:Tophive</span>
                </div>

            </div>

            <div class="my_card mb-3">

                <div class="mb-3">
                    <img src="../../assets/img/6498.jpg" alt="">
                </div>

                <div class="text-start px-2">
                    <span class="mb-3">$32.00</span>   
                    <h3 class="mb-3">CompTIA Network+ Cert. (N10-007)</h3>
                    <p class="mb-3">CompTIA Network+ (N10-007) Bootcamp - Certification preparation course on the most popular networking certification!</p>
                    <span class="author">Course by:Tophive</span>
                </div>

            </div>
    </div>
</template>
<script>
export default {
    name:"RecentCourses"
}
</script>
<style lang="scss" scoped>
img{
    width: 100%;
}
.title{
        p{
       width:65%;
       font-size: 0.9rem;
       margin: 0 auto; 
    }
}
.author{
    font-size: 0.7rem;
    color: red;
}
</style>