<template>
    <header >
    <nav class="container">
     
        <!-- logo dell'azienda -->
        <img src="../assets/logo.png" alt="">
      

      <ul class="navbar-links">
        <li v-for="(link, i) in links" :key="i">
          <a class="nav-link" href="">
            <i class="fas" :class="'fa-' + link.icon"></i>
            {{ link.text }}
          </a>
        </li>
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

<style lang="scss">
@use "../styles/partials/variables" as *;

header {
  background-color: $color-navbar-bg;
}

nav{
    display: flex;
   justify-content: space-between;
    align-items: center;
   
}
nav img{
    display: inline-block;
    padding: 0.5rem 1rem;
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


</style>