<template>
  <PageHeader :links="navLinks"/>
  <PageMain/>
  <PageFooter/>
  
</template>

<script>
import PageHeader from './components/PageHeader.vue';
import PageMain from './components/PageMain.vue';
import PageFooter from './components/PageFooter.vue';
import Jumbotron from './components/Jumbotron.vue';
import FaturedArticle from './components/FaturedArticle.vue';
import LatestNews from './components/LatestNews.vue';
import LatestNews2 from './components/LatestNews2.vue';
import TituralGuides from './components/TituralGuides.vue';
import ForumSections from './components/ForumSections.vue';
import Jumbotron2 from './components/Jumbotron2.vue';
export default{
  components: {
    PageHeader,
    PageMain,
    PageFooter,
    Jumbotron,
    FaturedArticle,
    LatestNews,
    LatestNews2,
    TituralGuides,
    ForumSections,
    Jumbotron2
    
    
  },
    data(){
      return {
        navLinks: [
        {
          href: "#home",
          text: "Home",
         
        },
        {
          href: "#apple",
          text: "Apple",
         
        },
        {
          href: "#microsoft",
          text: "Microsoft",
         
        },
        {
          href: "#android",
          text: "Android",
         
        },
        {
          href: "#contact us",
          text: "Concatct us",
         
        },
        {
          href: "#join us",
          text: "Join us",
          sticky: true
         
        },
        {
          icon: "magnifying-glass"
        },
      ],
      }

        
    }
}

</script>

<style lang="scss">
 @use "./styles/general.scss";
 .container{
  max-width: 1170px;
  margin: auto;
 }

</style>