<template>
  <div id="app">
    <Header/>

  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Service_section from "@/components/Service_section.vue";

export default {
  name: 'App',
  components: {
    Header,
    Service_section
  }
}
</script>

<style lang="scss">

*{
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}

</style>
