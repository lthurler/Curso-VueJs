<template>
  <main>
    <Navbar :logo="logo_scr" :alt="alt_name"/>
    <router-view/>
    <Footer /> 
  </main>  
</template>

<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'

export default {
  // name: 'App',
  components: {
    Navbar,
    Footer
  },
  
  data() {
    return {
      logo_scr: '/img/logo.png',
      alt_name: 'Make your burguer'
    }
  }

}
</script>

<style>
  * {
    font-family: Helvetica;
    margin:0;
    padding: 0;
    box-sizing: border-box;
  }  

  .main-container {    
    margin: 50px;
    min-height: 250px;
  }  

  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }

</style>
