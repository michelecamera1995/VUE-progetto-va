<template>
  <div id="app">
    <Header :menu="menu" />
    <Servicesection />
    <Skillsection />
    <Trustedsection />
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Servicesection from "@/components/Servicesection.vue";
import Skillsection from "@/components/Skillsection.vue";
import Trustedsection from "@/components/Trustedsection.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "App",
  data() {
    return {
      menu: [
        { name: "Home" },
        { name: "About" },
        { name: "Services" },
        { name: "Journal" },
        { name: "Contact" },
      ],
    };
  },
  components: {
    Header,
    Servicesection,
    Skillsection,
    Trustedsection,
    Footer,
  },
};
</script>

<style lang="scss">
* {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

*ul {
  list-style: none;
  text-decoration: none;
  display: flex;
}

*h6 {
  color: orange;
}

.button {
  padding: 10px 30px;
  font-size: 0.8rem;
  color: #60639b;
  font-weight: bold;
  cursor: pointer;
  border-radius: 7px;
}

.bt-or {
  background-color: #f86635;
  color: white;
}

.container {
  width: 1200px;
  margin: 0 auto;
}
</style>
