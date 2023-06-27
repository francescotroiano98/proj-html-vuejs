<template>
    <div class="jumbotron">
        
        <img :src="getImagePath(jumbotronimage[activeIndex])" alt="">
        <div class="learn-more text-center">

            <h1>Professional Development For Coaches And Leaders</h1>
            <button>Lear more</button>

        </div>    
           

        <button class="left" @click="previousSlide()">left</button>

        <button class="right" @click="nextSlide()">right</button>
    </div>
</template>
<script>
export default {
    name:"TopCarousel",
   

    data(){
        return{
            jumbotronimage:['jumbotron_1.PNG','jumbotron_2.PNG'],
            activeIndex : 0,
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

    .jumbotron{
        position: relative;
        height: 750px;
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
            bottom: 50%;
            left: 30%;
            width: 600px;
        
        }
        h1{

        }
        img{
            width:  100vw;
            height: 100%;
            object-fit: cover;
            

        }
    }
    
</style>