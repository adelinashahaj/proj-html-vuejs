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
            <input type="text" placeholder="Insert your email*" class="keyboard" v-model="newTask">
            <button class=" text-white bgcolor-btn rounded-0 " @click="addTask">SEND</button>
            <div v-show="error" class="error " >Errore, il testo deve essere lungo almeno 5 caratteri!</div>
                            
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
    components: { FaturedArticle, LatestNews, LatestNews2, TituralGuides, ForumSections, Jumbotron2 },
    data(){
        return{
            newTask: "",
            error: false,
            taskList: [
                
            ]
        }

    },
    methods: {
        addTask(){

            if(this.newTask.length >= 5){
                this.taskList.push(this.newTask);
                this.newTask= "";
                this.error = false;
            }else{
                this.error = true;
            }
          
        }
    }
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
        margin:  47px 0px 18px 0px;
       font-weight: bold;
       color: #535455;
       letter-spacing: 5px;
       font-size: 11px;
    }
    & h3{
        margin-bottom: 55px;
    }
}
.bgcolor-btn{
    background-color: $color-secondary;
    margin-left: 50px;
    padding: 8px 55px;
    font-weight: bold;
    border: none;
   
   }
   .keyboard{
    padding: 7px;
    min-width: 490px;
    border: 1px solid #bababa;
   }
   .error{
    color: red;
    text-align: center;
   }
.color-buttone{
    background-color: $color-secondary;
    font-weight: bold;
   
} 
</style>