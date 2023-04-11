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
     <section class="call_to_action  py-5">
        <LatestNews/>
        
    </section>

 <!--la terza sezione fattured article-->

    <section id="fattured">
        <FaturedArticle/>

    </section>
<!--la quarta sezione latest news2-->
    <section class="call_to_action  py-5">
        <LatestNews2/>
        
    </section>

    <!--la quinta sezione tutorials&guides-->
    <div class="container">
        <div class="row g-0 ">
            <div class="col-sm-6 col-md-8">
                <div class="fatturate2-img">
                <div class="text-fatured">
                    <p>FATURED ARTICLE</p>
                    <h1>Cras malesuada et orci eget pharetra</h1>
                    <p>Discuss all thr latest technology news and trends</p>
                    <a href="#" class="btn text-white color-btn rounded-0 ">READ MORE</a>
                            
                </div>
                </div>
            </div>
            <div class="col-6 col-md-4">
                <h4>Titural&Guides</h4>
                <div class="img-guides">
                    <img src="../assets/post_feat_img_23-147x118.jpg" alt="">
                    <div class="text-guides">
                        <h5>Donec ornare pretium eget scelisque justo</h5>
                    <p>October 11th, 2015 | Comments Off</p>
                    </div>
                    
                </div>
                <div class="img-guides">
                    <img src="../assets/post_feat_img_22-147x118.jpg" alt="">
                    <div class="text-guides">
                        <h5>Donec ornare pretium eget scelisque justo</h5>
                    <p>October 11th, 2015 | Comments Off</p>
                    </div>
                    
                </div>
                <div class="img-guides">
                    <img src="../assets/post_feat_img_20-147x118.jpg" alt="">
                    <div class="text-guides">
                        <h5>Donec ornare pretium eget scelisque justo</h5>
                    <p>October 11th, 2015 | Comments Off</p>
                    </div>
                    
                </div>
                
               

            </div>
        </div>
    </div>
    


    

    
  
</template>

<script>
import FaturedArticle from './FaturedArticle.vue';
import LatestNews from './LatestNews.vue';
import LatestNews2 from './LatestNews2.vue';

export default{
    data() {
    },
    components: { FaturedArticle, LatestNews, LatestNews2 }
}

</script>

<style lang="scss">
@use "../styles/partials/variables" as *;
@use "bootstrap";
.section-info{
   background-color: $color-bg;
  
}
.container-info{
    max-width: 1170px;
    margin: auto;
    text-align: center;
    padding: 20px 0;
}


.fatturate2-img{
    background-image: url("../assets/featured_article_2_bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    height: 465px;
    & img{
            height: 100%;
        }
        .text-fatured{
        color: white;
        padding-top: 200px;
        padding-left: 50px;
       
    }
    .color-btn{
    background-color: $color-btn;
   
   }
}
.img-guides {
    display: flex;
    & img {
        margin-left: 34px;
        margin-bottom: 37px;
    }
    p{
        color: gray;
        font-size: 11px;
    }
    & h5{
        font-size: 17px;
    }
    
}

</style>