
<template>
    <div class="container">
            <h6>PHASELLUS EGET METUS</h6>
            <h1>All the latest news</h1>
            <div class="border-b"></div>
            <div class="row row-cols-3">
                <div class="col ">
                   
                    <img class="img-fluid" src="../assets/post_feat_img_25-700x441.jpg" alt="">
                    <h5>Morbi vitae dui euismod vulputate sollictudin</h5>
                    <p>October 11th, 2015 | <span class="cl-comm"> 2 Comments</span></p>
                    <p>Donec finibus sit amet arci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulm placerat metus mattis. Aenean dictum vutae nis!</p>
                    
                </div>
                <div class="col">
                    
                    <img class="img-fluid" src="../assets/post_feat_img_24-700x441.jpg" alt="">
                    <h5>Vivamus pellenteque, felis quis varius</h5>
                    <p>October 11th, 2015 | Comments Off</p>
                    <p>Donec finibus sit amet arci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulm placerat metus mattis. Aenean dictum vutae nis!</p>
                
                </div>
                <div class="col ">
                        
                    <img class="img-fluid" src="../assets/post_feat_img_23-700x441.jpg" alt="">
                    <h5>Vivamus pellenteque, felis quis varius</h5>
                    <p>October 11th, 2015 | Comments Off</p>
                    <p>Donec finibus sit amet arci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulm placerat metus mattis. Aenean dictum vutae nis!</p>
                    
                </div>
            </div>
        </div>
  
</template>

<script>

export default{
    name: "LatestNews",
    data(){
        
    }
}

</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "bootstrap";

.container{
    max-width: 1170px;
    margin: auto;
    & h6{
        text-align: center;
        letter-spacing: 5px;
        margin:  47px 0px 18px 0px;
       font-weight: bold;
       color: #535455;
       font-size: 11px;
    }
    & h1{
        text-align: center;
        font-weight: bold;
        
    }
    & p{
        color: gray;
        font-size: 13px;
    }
    & h5{
        margin-top: 15px;
        font-size: 18px;
        font-weight: bold;
    }
    .cl-comm{
        color: $color-secondary;
    }
    
    .border-b{
        border-bottom: 2px solid $color-orange;
        height: 13px;
        width: 73px;
        margin-bottom: 32px;
        margin-left: 47%;
        left: 30px;
       
    }
}

</style>