<template>
  <div class="container">
    <!--service-section-->
    <div id="service-section">
      <h6>Available services</h6>
      <!--top-service-section-->
      <div id="top-service-section">
        <div class="service-card">
          <h3>Answering phone calls</h3>
          <p>
            Elementum posuere mauris,ac ultricies eu orci massa at id tincidunt
          </p>
        </div>
        <div class="service-card">
          <h3>Basic data entry</h3>
          <p>
            Elementum posuere mauris,ac ultricies eu orci massa at id tincidunt
          </p>
        </div>
        <div class="service-card">
          <h3>Organizing calendar</h3>
          <p>
            Elementum posuere mauris,ac ultricies eu orci massa at id tincidunt
          </p>
        </div>
        <div class="service-card">
          <h3>Booking travels</h3>
          <p>
            Elementum posuere mauris,ac ultricies eu orci massa at id tincidunt
          </p>
        </div>
      </div>
      <!--bottom-service-section-->
      <div id="bottom-service-section">
        <div id="Left-bottom-service">
          <img src="@/assets/info-5-2x-600x648.png" alt="info" />
        </div>
        <div id="Right-bottom-service">
          <img src="@/assets/icon-1-2x-200x155.png" alt="info" />
          <h2>Find the ultimate virtual assistant for your business</h2>
          <p>
            Mauris aliquam libero,fermentum quis eros,massa saggittis.Lectus
            mattis elit purus venenatis
          </p>
          <div>
            <button class="button bt-or">What is a VA exactly?</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Servicesection",
};
</script>

<style lang="scss" scoped>
#service-section {
  margin: 80px 0px;
  color: #60639b;
  h6 {
    font-size: 1rem;
  }
  #top-service-section {
    margin: 5%;
    display: flex;
    justify-content: space-between;
    .service-card {
      border-radius: 15%;
      width: 150px;
      height: 150px;
      h3 {
        font-size: 1.5rem;
      }
      p {
        margin-top: 15px;
      }
    }
  }
  #bottom-service-section {
    display: flex;
    margin-top: 100px;
    #Right-bottom-service {
      margin-right: 5%;
      width: 60%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;

      h2 {
        margin-top: 70px;
        font-size: 1.9rem;
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
    #Left-bottom-service {
      img {
        height: 700px;
      }
    }
  }
}
</style>