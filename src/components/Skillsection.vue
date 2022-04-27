<template>
  <div class="container" id="skillsection">
    <!--skillsection-->
    <div id="skillsection">
      <!--top-skillsection-->
      <div id="top-skillsection">
        <p>Donec est tristique eu massa pellentesque</p>
        <h2>Higly-skilled, indipendent porfessional freelancer.</h2>
        <button class="button bt-or">What is a VA exactly?</button>
      </div>
      <!--bottom-skillsection-->
      <div id="bottom-skillsection">
        <div class="skill-card">
          <h4>1.</h4>
          <div>
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
            <p>
              Vitae blandit aliquet a donec at nunc risus, enim,ultricies.Risus
              egestas nisl nisl convallis purus
            </p>
            <a href="#">Learn more</a>
          </div>
        </div>
        <div class="skill-card">
          <h4>3.</h4>
          <div>
            <p>
              Vitae blandit aliquet a donec at nunc risus, enim,ultricies.Risus
              egestas nisl nisl convallis purus
            </p>
            <a href="#">Learn more</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Skillsection",
};
</script>

<style lang="scss" scoped>
#skillsection {
  color: white;
  background-color: #0d1267;
  background-image: url("@/assets/info-bg-3.svg");
  background-position: bottom;
  background-repeat: no-repeat;
  #top-skillsection {
    padding-top: 100px;
    text-align: center;
    h2 {
      display: flex;
      justify-content: center;
      font-size: 2.5rem;
      margin: 50px 0;
    }
  }
  #bottom-skillsection {
    display: flex;
    justify-content: space-around;
    padding-top: 80px;
    padding-bottom: 100px;
    .skill-card {
      color: white;
      padding: 3% 3%;
      display: flex;
      width: 25%;
      background-color: #000545;
      font-size: 0.9rem;
      h4 {
        font-size: 2.4rem;
      }
      div {
        padding-left: 5%;
        p {
          font-size: 0.9rem;
          margin-bottom: 15px;
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