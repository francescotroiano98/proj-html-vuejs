<template>
    <div class="gallery d-flex justify-content-between overflow-scroll">
      <img v-for="(image) in displayedImages" :src="getImagePath(image)" alt="">
    </div>
  </template>
  
  <script>
  export default {
    name: "BottomCarousel",
  
    data() {
      return {
        galleryimage: [
          'gallery-1-3.jpg',
          'gallery-1-3.jpg',
          'gallery-2-3.jpg',
          'gallery-2-3(1).jpg',
          'gallery-3-3.jpg',
          'gallery-3-3(1).jpg'
        ],
        currentIndex: 0,
        displayedImages: []
      };
    },
  
    methods: {
      getImagePath(img) {
        return new URL(`../../assets/img/${img}`, import.meta.url).href;
      },

     
        updateDisplayedImages() {
            const startIndex = this.currentIndex;
            const endIndex = (this.currentIndex + 4) % this.galleryimage.length;

                if (startIndex <= endIndex) {
                    this.displayedImages = this.galleryimage.slice(startIndex, endIndex);
                } else {
                    this.displayedImages = this.galleryimage.slice(startIndex).concat(this.galleryimage.slice(0, endIndex)); // concat mi permette di combinare i due array senza modificare quello esistente
                }
        }
    },
  
    mounted() {

      this.updateDisplayedImages();

      setInterval(() => {

        this.currentIndex++;

        if (this.currentIndex >= this.galleryimage.length) {

          this.currentIndex = 0;

        }
        this.updateDisplayedImages();
        
      }, 3000);
    }
  };
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