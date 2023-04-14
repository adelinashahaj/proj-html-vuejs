<template>
    <header >
    <nav class="container">
     
        <!-- logo dell'azienda -->
        <img src="../assets/logo.png" alt="">
      

      <ul class="navbar-links">
        <li v-for="(link, i) in links" :key="i">
          <a   class="nav-link" :class="link.sticky == true? 'triangolo': ''" href="">
            {{ link.text }}
          </a>
          
        </li>
       
        <a href="#"><button class=" text-white color-btn rounded-0 " >Join us</button></a>
        <a href="#"> <i class="fa-solid fa-magnifying-glass"></i></a>
       
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
.color-btn{
    background-color: black;
    margin-right: 36px;
    margin-left: 25px;
    padding: 5px 20px;
    font-family: 'Fira Sans', sans-serif;
    border: none;
   }
    .triangolo {
    position: relative;
}
.triangolo:after {
    width: 0;
    height: 0;
    border-left: 26px solid transparent;
    border-right: 26px solid transparent;
    border-top: 31px solid $color-navbar-bg;
    position: absolute;
    content: "";
    top: 62px;
    left: 15px;
}
</style>