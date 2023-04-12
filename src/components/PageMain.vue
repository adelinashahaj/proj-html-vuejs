<template>
    <!--la prima sezione dopo jumbotron-->
    <div class="section-info">
        <div class="container-info">
            <h5>AVADA FORUM IS THE PLACE TO BE</h5>
        <p>In quis lectus sed leo elementum faucibus in dapibus dictum. 
            <p>Nulla molestie tortor nec lectus venenatis, sed blandit dui finibus, <br>
            dolor at, bibendum purus. Donec vehicula nec tortor ac finibus.</p> 
        </p>
        </div>

    </div>
     <!--la seconda sezione latest news-->
     <section class="all-news  py-5">
        <LatestNews/>
        
    </section>

 <!--la terza sezione fattured article-->

    <section id="fattured">
        <FaturedArticle/>

    </section>
<!--la quarta sezione latest news2-->
    <section class="all-news  py-5">
        <LatestNews2/>
        
    </section>

    <!--la quinta sezione tutorials&guides-->
    <section class="tutorial">
        <TituralGuides/>
    </section>
      <!--la sesta sezione forum sections-->
      <section class="forum-sections">
        <ForumSections/>
      </section>
       <!--JUMBOTRON 2-->
       <section class="jumbotron2">
        <Jumbotron2/>
      </section>
      <!--sezione email-->
      <div class="section-info">
        <div class="container-info">
            <h3>Subscribe to our Newsletter</h3>
            <input type="text" placeholder="Insert your email*" class="keyboard" >
            <a href="#" class="btn text-white bg-btn rounded-0 ">SEND</a>
                            
        </div>

    </div>


    

    
  
</template>

<script>
import FaturedArticle from './FaturedArticle.vue';
import ForumSections from './ForumSections.vue';
import Jumbotron2 from './Jumbotron2.vue';
import LatestNews from './LatestNews.vue';
import LatestNews2 from './LatestNews2.vue';
import TituralGuides from './TituralGuides.vue';



export default{
    name: "PageMain",
    data() {
    },
    components: { FaturedArticle, LatestNews, LatestNews2, TituralGuides, ForumSections, Jumbotron2 }
}

</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

.section-info{
   background-color: $color-bg;
  
}
.container-info{
    max-width: 1170px;
    margin: auto;
    text-align: center;
    padding: 36px 0;
    & p{
        color: gray;
       
    }
    & h5{
        padding-top: 10px;
    }
    & h3{
        margin-bottom: 55px;
    }
}
.bg-btn{
    background-color: $color-secondary;
    margin-left: 50px;
    padding: 8px 55px;
   
   }
   .keyboard{
    padding: 7px;
    min-width: 490px;
   }

</style>