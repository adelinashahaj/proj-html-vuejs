<template>
    <div class="jumbo-img">
       <div class="text-jumbotron">
        <h1>Tech Forum!</h1>
        <p>Discuss all thr latest technology news and trends</p>
        <a href="#" class="btn text-white color-btn rounded-0 ">GET AVADA NOW!</a>
                
       </div>
       
    </div>
    
    

</template>

<script>
export default{
}
</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "bootstrap";
.jumbo-img{
  background-image: url("../../public/home_slider_bg.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  height: 465px;
    & img{
        height: 100%;
    }
    .text-jumbotron{
        color: white;
        position: absolute;
        left: 23%;
        top: 29%;
    }
   .color-btn{
    background-color: $color-primary;
   
   }
  
}
</style>