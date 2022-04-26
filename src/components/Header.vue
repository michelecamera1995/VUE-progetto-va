<template>
  <div id='Header' >
    <div>
        <div id="Top-header"></div>
    </div>
        <div>
        <div id="Bottom-header"  class='container'></div>
    </div>
        
  </div>
</template>

<script>
export default {
name: 'Header',
}
</script>

<style lang="scss" scoped>

.container{
  width: 1200px;
  margin: 0 auto;
}

#Header{
    height: 700px;
    background-color: #0f1164;
    background-image: url('@/assets/info-bg-2.svg');
     #Top-header{
          width: 100%;
          height: 120px;
          background-color: yellow;
      }
      #Bottom-header{
          width: 1200px;
          height: 300px;
          margin: 0 auto;
          background-color: rgb(255, 0, 212);
      }
}

</style>