<template>
 <Navbar :logo="logo_src" :alt="app_name"/>
  <router-view/>
  <Footer/>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Footer from './components/Footer.vue'

export default {
    components: {
      Navbar,
      Footer
    },
    data() {
      return {
        logo_src: "/img/logo.png",
        app_name: "Make Your Burguer"
      }
    }
}
</script>


<style>
* {
  font-family: helvetica;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
/* falando de tudo, arrumou todas as letras para a mesma */
.main-container {
  margin: 50px;
  min-height: 250px;
}
/* da espaçamento entre as partes  */
h1{
  font-size: 42px;
  text-align: center;
  margin-bottom: 30px;
  color: #222;
}
/* falando de todos os h1 do projeto */
</style>
