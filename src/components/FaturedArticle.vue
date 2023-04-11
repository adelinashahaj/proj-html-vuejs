<template>
    <section id="fattured">
        <div class="container">
            <div class="fatturate-img">
                <div class="text-fatured">
                    <p>FATURED ARTICLE</p>
                    <h1>Cras malesuada et orci eget pharetra</h1>
                    <p>Discuss all thr latest technology news and trends</p>
                    <a href="#" class="btn text-white color-btn rounded-0 ">READ MORE</a>
                            
                </div>
        
            </div>

        </div>

    </section>
    
    

</template>

<script>
export default{

}
</script>

<style lang="scss"  >
@use "../styles/partials/variables" as *;
@use "bootstrap";

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
       
    }
    .color-btn{
    background-color: $color-btn;
   
   }
}

</style>