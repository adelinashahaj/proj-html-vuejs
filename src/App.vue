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
export default{
  components: {
    PageHeader,
    PageMain,
    PageFooter,
    Jumbotron
    
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