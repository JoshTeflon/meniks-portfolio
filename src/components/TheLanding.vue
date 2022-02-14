<script>
import HeroImage from "./HeroImage.vue";
import HeroItems from "./HeroItems.vue";
// import Nav from "./Nav.vue"

export default {
  name: "TheLanding",
  components: {
    HeroImage,
    HeroItems,
    // Nav,
  }
}

</script>

<template>
  <div class="landing">
    <!-- <Nav /> -->
    <div class="landing-content--wrapper">
      <div class="landing-content">
        <div class="hero--items">
          <HeroItems />
        </div>
        <div class="hero--image">
          <HeroImage />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
  .landing {
    margin: 0 auto;
    width: 80%;
    height: 85vh;
  }

  .landing .landing-content--wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    /* height: 100vh; */
  }

  .landing .landing-content--wrapper .landing-content {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    /* padding: 1rem 0; */
  }

  .landing .hero--items {
    width: 100%;
    margin: 0 0 3rem 0;
  }

  @media screen and (min-width: 640px) {
    .landing .landing-content--wrapper .landing-content {
      flex-direction: row;
      justify-content: space-between;
    }

    .landing .hero--items {
      width: 75%;
      margin: 0;
    }
  }
</style>
