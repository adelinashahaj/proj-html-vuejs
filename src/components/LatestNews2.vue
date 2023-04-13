<template>
    <div class="container">
        <div class="row row-cols-3">
                <div class="col ">
                   
                    <img class="img-fluid" src="../assets/post_feat_img_22-700x441.jpg" alt="">
                    <h5>Morbi vitae dui euismod vulputate sollictudin</h5>
                    <p>October 11th, 2015 | Comments Off</p>
                    <p>Donec finibus sit amet arci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulm placerat metus mattis. Aenean dictum vutae nis!</p>
                    
                </div>
                <div class="col">
                    
                    <img class="img-fluid" src="../assets/post_feat_img_21-700x441.jpg" alt="">
                    <h5>Vivamus pellenteque, felis quis varius</h5>
                    <p>October 11th, 2015 | Comments Off</p>
                    <p>Donec finibus sit amet arci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulm placerat metus mattis. Aenean dictum vutae nis!</p>
                
                </div>
                <div class="col ">
                        
                    <img class="img-fluid" src="../assets/post_feat_img_20-700x441.jpg" alt="">
                    <h5>Vivamus pellenteque, felis quis varius</h5>
                    <p>October 11th, 2015 | Comments Off</p>
                    <p>Donec finibus sit amet arci eget ultricies. Praesent posuere ante ut erat fringilla, vestibulm placerat metus mattis. Aenean dictum vutae nis!</p>
                    
                </div>
            </div>
    </div>
   
  
</template>

<script>

export default{
    name: "LatestNews2",
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
    & h6, h3{
        text-align: center;
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

}


</style>