<template>
  <div class="container" id="trusted">
    <!--brands-->
    <div id="brands">
      <h6>Trusted by these amazing brands</h6>
      <div id="brands-img">
        <img src="@/assets/brand-1-200x67.jpg" alt="brand1" />
        <img src="@/assets/brand-3-200x67.jpg" alt="brand1" />
        <img src="@/assets/brand-4-200x67.jpg" alt="brand1" />
        <img src="@/assets/brand-5-200x67.jpg" alt="brand1" />
        <img src="@/assets/brand-7-200x67.jpg" alt="brand1" />
      </div>
    </div>
    <!--top-trusted-->
    <div id="top-trusted">
      <div id="top-trusted-section">
        <div id="Left-top-trusted">
          <img src="@/assets/icon-2-2x-200x127.png" alt="info" />
          <h2>Profesional who works to help with your business.</h2>
          <p>
            Mauris aliquam libero,fermentum quis eros,massa saggittis.Lectus
            mattis elit purus venenatis
          </p>
          <div>
            <button class="button bt-or">What is a VA exactly?</button>
          </div>
        </div>
        <div id="Right-top-trusted">
          <img src="@/assets/info-8-2x-600x610.png" alt="info" />
        </div>
      </div>
    </div>
    <!--bottom-trusted-->
    <div id="bottom-trusted">
      <div class="skill-card">
        <h4>1.</h4>
        <div>
          <h5>Learn to delegate</h5>
          <p>
            Vitae blandit aliquet a donec at nunc risus, enim,ultricies.Risus
            egestas nisl nisl convallis purus
          </p>
          <a href="#">Learn more</a>
        </div>
      </div>
      <div class="skill-card">
        <h4>2.</h4>
        <div>
          <h5>Reduce labor costs</h5>
          <p>
            Vitae blandit aliquet a donec at nunc risus, enim,ultricies.Risus
            egestas nisl nisl convallis purus
          </p>
          <a href="#">Learn more</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Trustedsection",
};
</script>

<style lang="scss" scoped>
#trusted {
  #brands {
    display: flex;
    align-items: center;
    flex-direction: column;
    margin-top: 100px;
    margin-bottom: 100px;
    h6 {
      text-align: center;
      font-size: 1rem;
    }
    #brands-img {
      margin-top: 20px;
    }
  }
  #top-trusted-section {
    display: flex;
    margin-top: 100px;
    #Left-top-trusted {
      margin-right: 5%;
      width: 60%;
      display: flex;
      flex-direction: column;
      color: #60639b;
      justify-content: center;
      align-items: center;
      h2 {
        margin-top: 70px;
        font-size: 40px;
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
    #Right-top-trusted {
      img {
        height: 700px;
      }
    }
  }
  #bottom-trusted {
    display: flex;
    padding-top: 80px;
    justify-content: space-around;
    padding-bottom: 100px;
    .skill-card {
      color: white;
      padding: 3% 3%;
      display: flex;
      width: 45%;
      background-color: #0d1267;
      font-size: 0.9rem;
      h4 {
        font-size: 2.4rem;
      }
      div {
        padding-left: 5%;
        h5 {
          font-size: 1.1rem;
        }
        p {
          font-size: 0.9rem;
          margin: 15px 0;
        }
        a {
          color: #f86635;
          padding-top: 50px;
        }
      }
    }
  }
}
</style>