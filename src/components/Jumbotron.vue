<template>
    <div class="jumbo-img">
       <div class="text-jumbotron">
            <h1>Tech Forum!</h1>
            <p>Discuss all thr latest technology news and trends</p>
            <a href="#" class="btn text-white color-btn rounded-0 ">GET AVADA NOW! <i class="fa-solid fa-angle-right fnt-size"></i></a>
                
       </div>
       
    </div>
    
    

</template>

<script>
export default{
    name: "Jumbotron",
    data(){

    }
}
</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

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
        max-width: 1170px;
        margin: auto;
        padding-top: 146px;
        padding-left: 26px;
        & h1{
            font-size: 70px;
        }

    }
   .color-btn{
    background-color: $color-primary;
    font-weight: bold;
   
   }
  
}
.fnt-size{
    font-size: 13px;
}
</style>