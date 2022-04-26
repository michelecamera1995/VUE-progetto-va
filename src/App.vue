<template>
  <div id="app">
    <Header/>
    <Servicesection/>
    <Skillsection/>
    <Trustedsection/>
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Servicesection from "@/components/Servicesection.vue";
import Skillsection from "@/components/Skillsection.vue";
import Trustedsection from "@/components/Trustedsection.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: 'App',
  data(){
    return{
      menu : ['Home','About','Services','Journal','Contact']
    }
  },
  components: {
    Header,
    Servicesection,
    Skillsection,
    Trustedsection,
    Footer
  }
}
</script>

<style lang="scss">

*{
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

.container{
  width: 1200px;
  margin: 0 auto;
}

</style>
