<template>
    <div class="gallery d-flex justify-content-between overflow-scroll">
        
        <img v-for="(image, index) in galleryimage" v-show="index < 4" :src="getImagePath(image)" alt="">
        
        

    </div>
    
</template>
<script>
export default {
    name:"BottomCarousel",

    data(){
        return{
            galleryimage:['gallery-1-3.jpg','gallery-1-3.jpg','gallery-2-3.jpg','gallery-2-3(1).jpg','gallery-3-3.jpg','gallery-3-3(1).jpg'],
            activeIndex : 0,
            autoplay: false
        }
    },

    methods: {
        getImagePath:function(img){
            return new URL(`../../assets/img/${img}`, import.meta.url).href
        },

        previousSlide(){
        if(this.activeIndex === 0){

            this.activeIndex = this.galleryimage.length - 1;

        } else {

            this.activeIndex--;
        }
    },
    nextSlide() {

        if(this.activeIndex === this.galleryimage.length - 1){

            this.activeIndex = 0

        } else {
            this.activeIndex++;
        }
    },
    },
    mounted() {
        this.autoplay = setInterval(this.nextSlide, 3000);
    },
   
}
</script>
<style lang="scss" scoped>

.gallery{
        position: relative;
        height: 300px;
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
        .gallery{
            width: 100%;
        
                
        }
        img{
                    width:calc((100vw /4.2));
                    margin-right: 0.5rem ;
                    margin-left: 0.5rem;
                    height: 100%;
                    object-fit: cover;
                }
    }
</style>    