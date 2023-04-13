<template>
   
    <div class="bg-color">
        <div class="bg-black">
          <h6>READ OUR BLOG &rarr;</h6>

         </div>
        <div class="container">
            <h4 class="text-center">PHASELLUS EGET METUS</h4>
            <h1 class="text-center">Forum Sections</h1>
            <div class="border-b"></div>
            <div class="row-1 " >
                
                <div class="col-2" v-for="(icons, i) in iconsList" :key="i">
                    <div class="circle-orange" >

                        <i :class="icons.family == true? 'fab fa-'+ icons.icon : 'fas fa-'+ icons.icon" ></i>
    
                    </div>
                    <h5>{{ icons.text }}</h5>
                    
                </div>
                
                
            </div>
           

        </div>
        <div class="bg-black">
          <h6>GET TO OUR FORUM &rarr;</h6>

         </div>
    </div>
    
  
</template>

<script>

export default{
    name: "ForumSections",
    data(){
        
        return {
            iconsList: [
                {
                    text: "News & Community",
                    icon: "file",
                    family: "fas",
                },
                {
                    text: "Apple Forum",
                    icon: "apple",
                    family: true,
                },
                {
                    text: "Microsoft Forum",
                    icon: "microsoft",
                    family: true,
                },
                {
                    text: "Android Forum",
                    icon: "android",
                    family: true,
                },
                {
                    text: "General Discussion",
                    icon: "mug-saucer",
                    family: "fas",
                },
                {
                    text: "Apps & Software",
                    icon: "shapes",
                    family: "fas",
                },
                {
                    text: "Gadgets & Stuff",
                    icon: "laptop",
                    family: "fas",
                },
                {
                    text: "Tutorials & Guides",
                    icon: "wrench",
                    family: "fas",
                },
            ]
        }
        
    }
}

</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;



.bg-color{
    background-color: $color-bg;
    .bg-black {
    height: 70px;
    color: white;
    text-align: center
  }
     & h6{
        margin-top: 30px;
        font-size: 13px;
        padding-top: 25px;
        font-weight: bold;

    }
}
.container{
    max-width: 1170px;
    margin: auto;

    .border-b{
        border-bottom: 2px solid $color-orange;
        height: 13px;
        width: 73px;
        margin-bottom: 32px;
        margin-left: 47%;
        left: 30px;
       
    }
    & h1{
        font-weight: bold;
    }
}
.col-2{
  
    margin: 20px;
    height: 165px;
    border-top: 2px solid rgb(24, 189, 211);
    background-color: white;
    .circle-orange{
        border-radius: 50px;
        background-color: $color-orange;
        border-radius: 50px;
        height: 50px;
        width: 50px;
        text-align: center;
        color: white;
        padding-top: 5px;
        margin-left: 66px;
        margin-top: 30px;
        font-size: 26px;

    }
    & h5{
        font-size: 16px;
        text-align: center;
        margin-top: 5px;
        font-weight: bold;
    }

}
.row-1{
   justify-content: space-between;
    display: flex;
    flex-wrap: wrap;
}
h4{
    margin:  100px 0px 18px 0px;
       font-weight: bold;
       color: #535455;
       letter-spacing: 5px;
       font-size: 11px;
}

</style>