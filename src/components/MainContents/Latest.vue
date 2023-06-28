<template>
    <div class="title text-center mb-5">
        <h2 class="mb-3">Latest From Our Blogs</h2>
        <p>Whether you're considering a foundation course or an undergraduate degree master's or a PhD, academics is a place where students thrive.</p>
    </div>
    <div class="d-flex flex-wrap justify-content-between mb-5">
           
           <div class="my_card mb-3">

                <div class="mb-3">
                    <img src="../../assets/img/news-3-2.jpg" alt="">
                </div>
                
                <div class="text-start px-4">
                    <div class="d-flex">
                        <div class="d-flex align-items-center me-2">
                            <i class="fa-regular fa-user me-2" style="color: #b6bdc8;"></i><a href="#">Tophive</a>
                        </div>
                        <div class="d-flex align-items-center ">
                            <i class="fa-regular fa-folder me-2" style="color: #bdbfc1;"></i> <a href="#">University</a>
                        </div>

                    </div>
                    
                    <h3 class="mb-3">Peer pressure changes how teens tackle inequality</h3>
                    
                    <div class="line mb-5">

                    </div>

                    <div class="align-self-center">
                        <p class="learn-more">Event Locations</p>
                    </div>

                </div>

            </div>
            
            <div class="my_card mb-3">

                <div class="mb-3">
                    <img src="../../assets/img/news-2-2.jpg" alt="">
                </div>

                <div class="text-start px-4">
                    <div class="d-flex">
                        <div class="d-flex align-items-center me-2">
                            <i class="fa-regular fa-user me-2" style="color: #b6bdc8;"></i><a href="#">Tophive</a>
                        </div>
                        <div class="d-flex align-items-center ">
                            <i class="fa-regular fa-folder me-2" style="color: #bdbfc1;"></i> <a href="#">University</a>
                        </div>

                    </div>
                    
                    <h3 class="mb-3">Peer pressure changes how teens tackle inequality</h3>
                    
                    <div class="line mb-5">

                    </div>

                    <div class="align-self-center">
                        <p class="learn-more">Event Locations</p>
                    </div>

                </div>

            </div>

            <div class="my_card mb-3">

                <div class="mb-3">
                    <img src="../../assets/img/news-1-2.jpg" alt="">
                </div>

                <div class="text-start px-4">
                    <div class="d-flex">
                        <div class="d-flex align-items-center me-2">
                            <i class="fa-regular fa-user me-2" style="color: #b6bdc8;"></i><a href="#">Tophive</a>
                        </div>
                        <div class="d-flex align-items-center ">
                            <i class="fa-regular fa-folder me-2" style="color: #bdbfc1;"></i> <a href="#">University</a>
                        </div>

                    </div>
                    
                    <h3 class="mb-3">Peer pressure changes how teens tackle inequality</h3>
                    
                    <div class="line mb-5">

                    </div>

                    <div class="align-self-center">
                        <p class="learn-more">Event Locations</p>
                    </div>

                </div>

</div>
    </div>
</template>
<script>
export default {
    name:"Latest"
}
</script>
<style lang="scss" scoped>
.my_card{
    
    width: calc((100% / 3.3));
    box-shadow: rgba(0, 0, 0, 0.24) 0px 3px 8px;
    h3{
        font-size: 1.2rem;
        font-weight: 600;
    }
   p{
    font-size: 0.9rem;
    line-height: 1.6rem;
   }
    img{
        width: 100%;
        align-self: center;
    }
}
img{
    width: 100%;
}
.author{
    font-size: 0.7rem;
    color: red;
}
a{
    color: black;
    font-size: 0.8rem;
}
i{
    font-size: 0.7rem;
}
.line{
    height: 2px;
    background-color: red;
    width: 45px;
}
p.learn-more{
        font-weight: 700;
        font-size: 0.8rem;
    }    
</style>