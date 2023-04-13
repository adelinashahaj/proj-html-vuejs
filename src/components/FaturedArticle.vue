<template>
    <section id="fattured">
        <div class="container">
            <div class="fatturate-img">
                <div class="text-fatured">
                    <h6>FATURED ARTICLE</h6>
                    <h1>Cras malesuada et orci eget pharetra</h1>
                    <p>In quis lectus sed leo elementum faucibus in dapibus dictum. Nullamolestie tortor nec lectus venenatis, sed blandit dui,<br> dolor at bibendum sadips ets ipsums dolores ficilis uns leo lectus.</p>
                    <a href="#" class="btn text-white bg-btn rounded-0 ">READ MORE <i class="fa-solid fa-angle-right fnt-size"></i> </a>
                            
                </div>
        
            </div>

        </div>

    </section>
    
    

</template>

<script>
export default{
    name: "FaturedArticle",
    data(){

    }

}
</script>

<style lang="scss" scoped >
@use "../styles/partials/variables" as *;
@use "bootstrap";

.container{
    max-width: 1170px;
    margin: auto;
}
.fatturate-img{
    background-image: url("../assets/featured_article_1_bg.jpg");
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
        & h1{
            font-weight: bold;
        }
        & h6{
            letter-spacing: 5px;
        }
       
    }
    .bg-btn{
    background-color: $color-secondary;
    font-weight: bold;
   
   }
}
.fnt-size{
    font-size: 13px;
}

</style>