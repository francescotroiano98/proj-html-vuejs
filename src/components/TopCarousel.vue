<template>
    <div class="jumbotron">
        
        <img :src="getImagePath(jumbotronimage[activeIndex])" alt="">

        <div class="learn-more text-center" v-if="activeIndex === 0">
            <h1>
                Professional Development For Coaches And Leaders
            </h1>
        <button class="border-0 py-2 px-3">Learn More</button>
    </div>

    <div class="learn-more-1 text-center" v-if="activeIndex === 1">

      <h1>Experience The Next Level Of Coaching Education</h1>
      <button class="learn border-0 py-2 px-3">Learn More</button>

    </div>   
           

        <button class="left rounded-5" @click="previousSlide"><i class="fa-solid fa-chevron-left" style="color: #d1d1d1;"></i></button>

        <button class="right rounded-5" @click="nextSlide()"><i class="fa-solid fa-chevron-right" style="color: #bababa;"></i></button>
    </div>
</template>
<script>
export default {
    name:"TopCarousel",
   

    data(){
        return{
            jumbotronimage:['jumbotron_1.PNG','jumbotron_2.PNG'],
            activeIndex : 0,
            autoplay: false,
        }
    },

    methods: {
        getImagePath:function(img){
            return new URL(`../assets/img/${img}`, import.meta.url).href
        },

        previousSlide(){
        if(this.activeIndex === 0){

            this.activeIndex = this.jumbotronimage.length - 1;

        } else {

            this.activeIndex--;
        }
    },
    nextSlide() {

        if(this.activeIndex === this.jumbotronimage.length - 1){

            this.activeIndex = 0

        } else {
            this.activeIndex++;
        }
        
    },
    },
}
</script>
<style lang="scss" scoped>
h1{
    font-family: 'Times New Roman', Times, serif;
    margin-bottom: 2rem;
}
button{
        background-color: white;
    
        box-shadow: rgba(0, 0, 0, 0.15) 0px 3px 8px;
    }
    .learn-more-1 button:hover{
        background-color: #ff5166;
        color: white;
    }
    .learn-more button:hover{
        background-color: #ff5166;
        color: white;
    }
    .left{
        height: 60px;
        width: 60px;
    }
    .left:hover {
        
        background-image: url('../assets/img/jumbotron_2.PNG');
        background-size: cover;
        background-position: center;
        
    }
    .right:hover {
        
        background-image: url('../assets/img/jumbotron_2.PNG');
        background-size: cover;
        background-position: center;
        
    }
    .right{
        height: 60px;
        width: 60px;
    }
    .jumbotron{
        position: relative;
        height: 850px;
        width: 100%;
        background-color: greenyellow;
        margin-bottom: 2rem;
        
        button.left{
            position:absolute;
            left: 10px;
            top: 50%;
        }
        button.right{
            position:absolute;
            right: 10px;
            top: 50%;
        }
        .learn-more{
            position: absolute;
            bottom: 55%;
            left: 30%;
            width: 600px;
        
        }
        .learn-more-1{
            position: absolute;
            bottom: 72%;
            left: 30%;
            width: 600px;
        }
        img{
            width:  100vw;
            height: 100%;
            object-fit: cover;
            

        }
    }
    
</style>