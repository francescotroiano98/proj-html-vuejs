<template>
    <div class="text-center mb-5">
        <h2>Since 2000, weve been partnering with educational leaders to <span>increase equity and achievement</span> for all student</h2>
    </div>
    <div class="d-flex flex-wrap justify-content-between mb-5">
           
        <div class="my_card text-center py-5 px-4">
            <img class="mb-3" src="../../assets/img/svg-0.svg" alt="">
            <h3 class="mb-3">Online Coaching</h3>
            <p class="mb-3">Lorem ipsum is simply dummy text of the print ing and typesetting has been the industrys.</p>
        </div>
        <div class="my_card text-center py-5 px-4">
            <img class="mb-3" src="../../assets/img/svg-1.svg" alt="">
            <h3 class="mb-3">Consultation</h3>
            <p class="mb-3">Lorem ipsum is simply dummy text of the print ing and typesetting has been the industrys.</p>
        </div>
        <div class="my_card text-center py-5 px-4">
            <img class="mb-3" src="../../assets/img/svg-2.svg" alt="">
            <h3 class="mb-3">Life Programs</h3>
            <p class="mb-3">Lorem ipsum is simply dummy text of the print ing and typesetting has been the industrys.</p>
        </div>
        
    </div>
    <div class="d-flex justify-content-between mb-5">
        <div><h2>{{ counterStudents }}</h2></div>
        <div><h2>{{ counterCourses }}</h2></div>
        <div><h2>{{ counterHappyClients }}</h2></div>
    </div>
    
</template>
<script>
export default {
    name:"Description",
    data(){
        return{
            counterStudents:1000,
            counterCourses:0,
            counterHappyClients:0
        }
    },
    mounted() {
    const interval1 = setInterval(() => {
      this.counterStudents = this.counterStudents + 100;
      if (this.counterStudents >= 6500) {
        clearInterval(interval1);
      }
    }, 50);

    const interval2 = setInterval(() => {
      this.counterCourses++;
      if (this.counterCourses >= 200) {
        clearInterval(interval2);
      }
    }, 10);

    const interval3 = setInterval(() => {
      this.counterHappyClients++;
      if (this.counterHappyClients >= 100) {
        clearInterval(interval3);
      }
    }, 20);
  }

}
</script>
<style lang="scss">

.my_card{
    
    width: calc((100% / 3.5));
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
        width: 50px;
        align-self: center;
    }
}
    
</style>