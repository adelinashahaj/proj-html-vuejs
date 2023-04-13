<template>
    <header >
    <nav class="container">
     
        <!-- logo dell'azienda -->
        <img src="../assets/logo.png" alt="">
      

      <ul class="navbar-links">
        <li v-for="(link, i) in links" :key="i">
          <a   class="nav-link" :class="link.sticky == true? '': ''" href="">
            {{ link.text }}
          </a>
          
        </li>
        <a href="#" class="btn text-white bg-btn rounded-0 ">Join us</a>
        <a href=""> <i class="fa-solid fa-magnifying-glass"></i></a>
       
      </ul>
     
                            
    </nav>
  </header>
  <div>
    <Jumbotron/>
  </div>
  
</template>

<script>
import Jumbotron from './Jumbotron.vue';



export default{
    name: "PageHeader",
    data() {
        return {};
    },
    props: {
        links: Array
    },
    components: { Jumbotron }
}

</script>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;
@use "bootstrap";


header {
  background-color: $color-navbar-bg;
}
.container{
  max-width: 1170px;
  margin: auto;
}
nav{
    display: flex;
   justify-content: space-between;
    align-items: center;
   
}
nav img{
    display: inline-block;
  
}
.navbar-links { 
    display: flex;
    justify-content: end;
    align-items: center;
    list-style: none;
    padding-top: 15px;
}

a.nav-link {
    padding: 20px;
    color: white;
}
i {
   
    color: white;
}
.bg-btn{
    background-color: black;
    margin-right: 23px;
    padding: 5px 20px;
    font-family: 'Fira Sans', sans-serif;
   }


</style>