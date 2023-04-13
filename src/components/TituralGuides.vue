<template>
     <div class="container">
        <div class="row g-1">
            <div class="col-sm-6 col-md-8">
                <div class="fatturate2-img">
                <div class="text-fatured">
                    <h6>REVIEWED PRODUCT</h6>
                    <h1>Mauris viverra atisan ipsum eget felis prims efficitur varius</h1>
                    <p>In quis lectus sed leo elementum faucibus in dapibus dictum.
                     Nulla molestie tortor nec lectus venenatis, sed blandit dui, dolor at bibendum.</p>
                    <a href="#" class="btn text-white color-buttone rounded-0 ">READ MORE <i class="fa-solid fa-angle-right fnt-size"></i></a>
                            
                </div>
                </div>
            </div>
            <div class="col-6 col-md-4 px-3">
                <h4>Titural&Guides</h4>
                <div class="border-b"></div>
                <div class="img-guides">
                    <img src="../assets/post_feat_img_23-147x118.jpg" alt="">
                    <div class="text-guides">
                        <h6>Donec ornare pretium eget scelisque justo</h6>
                    <p>October 11th, 2015 | Comments Off</p>
                    </div>
                    
                </div>
                <div class="img-guides">
                    <img src="../assets/post_feat_img_22-147x118.jpg" alt="">
                    <div class="text-guides">
                        <h6>Donec ornare pretium eget scelisque justo</h6>
                    <p>October 11th, 2015 | Comments Off</p>
                    </div>
                    
                </div>
                <div class="img-guides">
                    <img src="../assets/post_feat_img_20-147x118.jpg" alt="">
                    <div class="text-guides">
                        <h6>Donec ornare pretium eget scelisque justo</h6>
                    <p>October 11th, 2015 | Comments Off</p>
                    </div>
                    
                </div>
                
               

            </div>
        </div>
    </div>
  
</template>

<script>

export default{
    name: "TituralGuides",
   
}

</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "bootstrap";

.container{
    max-width: 1170px;
    margin: auto;
}
.fatturate2-img{
    background-image: url("../assets/featured_article_2_bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    height: 465px;
    margin-top: 6px;
    & img{
            height: 100%;
        }
     .text-fatured{
        color: white;
         padding-top: 120px;
        padding-left: 50px;

        & h1 {
         font-weight: bold;
        }
        & h6{
            letter-spacing: 5px;
        }
            
    }
.color-buttone{
    background-color: $color-secondary;
    font-weight: bold;
   
}
}
.img-guides {
    display: flex;
    & img {
       
        margin-bottom: 30px;
    }
    p{
        color: gray;
        font-size: 11px;
    }
    & h6{
        font-size: 17px;
        font-weight: bold;
    }
    
}

.border-b{
    border-bottom: 2px solid $color-orange;
    height: 5px;
    width: 52px;
    margin-bottom: 15px;
}
.text-guides {
    margin-left: 10px;
}
.fnt-size{
    font-size: 13px;
}
h4{
    font-weight: bold;  
}

</style>