<template>
    <section id="fattured">
        <div class="container">
            <div class="fatturate-img">
                <div class="text-fatured">
                    <p>FATURED ARTICLE</p>
                    <h1>Cras malesuada et orci eget pharetra</h1>
                    <p>Discuss all thr latest technology news and trends</p>
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
            font-family: 'Fira Sans', sans-serif;
            font-weight: bold;
        }
        & p{
            font-family: 'Fira Sans', sans-serif;
        }
       
    }
    .bg-btn{
    background-color: $color-secondary;
    font-family: 'Fira Sans', sans-serif;
    font-weight: bold;
   
   }
}
.fnt-size{
    font-size: 13px;
}

</style>