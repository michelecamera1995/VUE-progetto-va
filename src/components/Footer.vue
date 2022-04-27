<template>
  <div class="bg-footer">
    <div id="top-footer" class="container">
      <!--Header Left-->
      <div id="left-Top-footer">
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
      <div id="right-Top-footer">
        <p>
          <i class="fa-solid fa-headphones"></i>
          1.800.123.4567
        </p>
        <button class="button">Get a free consultation!</button>
      </div>
      <!---->
    </div>
    <div id="bottom-footer" class="container">
      <h2>
        Indipendent professional who works remotely to help with your business.
      </h2>
      <div>
        <button class="button">What is a VA exactly?</button>
      </div>
      <p>
        @Copyright 2012-2020 | Avada theme | All rigths reserved | Powered by
        wordpress
      </p>
    </div>
  </div>
</template>

<script>
import Listcomponent from "@/components/Listcomponent.vue";
export default {
  name: "Footer",
  components: {
    Listcomponent,
  },

  props: {
    menu: Array,
  },
};
</script>

<style lang="scss" scoped>
.bg-footer {
  background-color: #0d1267;
}
#top-footer {
  height: 150px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
  #left-Top-footer {
    display: flex;
    img {
      margin-right: 5%;
    }
  }
  #right-Top-footer {
    display: flex;
    p {
      display: flex;
      align-items: center;
    }
    button {
      background-color: #000545;
      margin: 0px 70px;
      color: white;
    }
  }
}
#bottom-footer {
  display: flex;
  flex-direction: column;
  color: white;
  h2 {
    margin: 15px 0;
    width: 40%;
  }
  button {
    margin: 25px 0;
  }
  p {
    font-size: 0.7rem;
    margin-bottom: 50px;
  }
}
</style>