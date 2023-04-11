
<template>
    <div class="container">
            <h6>PHASELLUS EGET METUS</h6>
            <h3>All the latest news</h3>
            <div></div>
            <div class="row row-cols-3">
                <div class="col ">
                   
                    <img class="img-fluid" src="../assets/post_feat_img_25-700x441.jpg" alt="">
                    <h5>Morbi vitae dui euismod vulputate sollictudin</h5>
                    <p>October 11th, 2015 | 2 Comments</p>
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
    }
}

</style>