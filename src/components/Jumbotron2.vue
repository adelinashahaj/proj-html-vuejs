<template>
 <div class="jumbo-img">
       <div class="text-jumbotron">
            <h1>Hey! Join to our <br> Community</h1>
            <p>Nulla molestie tortor nec lectus venenatis, sed blandit dui finibus. 
                Curabitur feugiat <br> vulputate purus ipsums dolores ficilis un etra.</p>
            <a href="#" class="btn text-white color-btn rounded-0 ">SING UP! <i class="fa-solid fa-angle-right fnt-size"></i></a>
                
       </div>
       
    </div>

  
</template>

<script>
export default{
    name: "Jumbotron2",
    data(){
        
    }
}

</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.jumbo-img{
  background-image: url("../../public/join_now_cta_bg.jpg");
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
        text-align: center;
        & h1{
            font-size: 64px;
            font-family: 'Fira Sans', sans-serif;
        }
        & p{
            font-family: 'Fira Sans', sans-serif;
        }

    }
   .color-btn{
    background-color: $color-primary;
    font-family: 'Fira Sans', sans-serif;
    font-weight: bold;
   
   }
  
}
.fnt-size{
    font-size: 13px;
}
</style>