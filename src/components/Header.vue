<template>
  <div id='Header' >
    <div>
        <div id="Top-header">

            <!--Header Left-->
            <div id="Left-Top-header">
                <img src="@/assets/logo.png" alt="">
                <ul>
                    <Listcomponent v-for="(items,index) in menu" :key="index" :items="items"/>
                </ul>
            </div>
            <!---->

            <!--Header Right-->
            <div id="Right-Top-header">
                <p>1.800.123.4567</p>
                <button class="button">Get a free consultation!</button>
            </div>
            <!---->

        </div>
    </div>
        <div id="Bottom-header"  class='container'></div>
    </div>
        

</template>

<script>
import Listcomponent from "@/components/Listcomponent.vue";
export default {
name: 'Header',

components:{
    Listcomponent
},

props: {
    menu: Array,
},

}
</script>

<style lang="scss" scoped>

.container{
  width: 1200px;
  margin: 0 auto;
}

#Header{

    color: white;
    background-color: #0f1164;
    background-image: url('@/assets/info-bg-2.svg');
    font-weight: bold;

     #Top-header{
          width: 100%;
          height: 120px;
          display: flex;
          justify-content: space-between;
          align-items: center;

          #Left-Top-header{
              display: flex;
              img{
                  margin-left: 20%;
                  margin-right: 15%;
              }
          }

          #Right-Top-header{
              display: flex;
              p{
                  display: flex;
                  align-items: center;
              }
              button{
                  margin: 0px 70px
              }
          }
      }

      #Bottom-header{
          width: 1200px;
          height: 300px;
          margin: 0 auto;
      }
}

</style>