<template>
  <div id="Header">
    <div>
      <div id="Top-header">
        <!--Header Left-->
        <div id="Left-Top-header">
          <img src="@/assets/logo.png" alt="" />
          <ul>
            <Listcomponent
              v-for="(items, index) in menu"
              :key="index"
              :items="items"
            />
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
    <div id="Bottom-header" class="container">
      <div id="Left-Bottom-header">
        <h2>
          Indipendent professional who works remotely to help with your
          business.
        </h2>
        <p>
          Mauris aliquam libero,fermentum quis eros,massa saggittis.Lectus
          mattis elit purus venenatis
        </p>
        <div>
          <button class="button">What is a VA exactly?</button>
        </div>
      </div>
      <div id="Right-Bottom-header">
        <img src="@/assets/info-5-600x666.jpg" alt="info" />
      </div>
    </div>
  </div>
</template>

<script>
import Listcomponent from "@/components/Listcomponent.vue";
export default {
  name: "Header",

  components: {
    Listcomponent,
  },

  props: {
    menu: Array,
  },
};
</script>

<style lang="scss" scoped>
.container {
  width: 1200px;
  margin: 0 auto;
}

#Header {
  height: 700px;
  color: white;
  background-color: #0f1164;
  background-image: url("@/assets/info-bg-2.svg");
  background-position: center;
  font-weight: bold;

  #Top-header {
    width: 100%;
    height: 150px;
    display: flex;
    justify-content: space-between;
    align-items: center;

    #Left-Top-header {
      display: flex;
      img {
        margin-left: 20%;
        margin-right: 15%;
      }
    }

    #Right-Top-header {
      display: flex;
      p {
        display: flex;
        align-items: center;
      }
      button {
        margin: 0px 70px;
      }
    }
  }

  #Bottom-header {
    width: 1200px;
    margin: 0 auto;
    display: flex;

    #Left-Bottom-header {
      margin-right: 5%;
      width: 60%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      h2 {
        font-size: 50px;
        text-align: center;
      }
      p {
        margin: 8%;
        font-weight: 200;
        text-align: center;
      }
      button {
        text-align: center;
      }
    }
    #Right-Bottom-header {
      img {
        height: 580px;
      }
    }
  }
}
</style>