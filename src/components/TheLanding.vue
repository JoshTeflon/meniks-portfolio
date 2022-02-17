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
    width: var(--width-mobile);
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .landing .landing-content--wrapper {
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 8rem auto 4rem auto;
    /* height: 100vh; */
  }

  .landing .landing-content--wrapper .landing-content {
    width: 100%;
    display: flex;
    flex-direction: column-reverse;
    align-items: center;
    justify-content: center;
  }

  .landing .hero--items {
    width: 100%;
    margin: 1rem auto;
  }

  @media screen and (min-width: 640px) {
    .landing {
      width: var(--width-tablet);
      height: 100vh;
    }

    .landing .landing-content--wrapper {
      margin: 0 auto;
    }

    .landing .landing-content--wrapper .landing-content {
      flex-direction: row;
      justify-content: space-between;
      padding-top: 4rem;
    }

    .landing .hero--items {
      width: 95%;
      margin: 0;
    }
  }

  @media screen and (min-width: 1024px) {
    .landing {
      width: var(--width-tablet-lg);
    }
  }

  @media screen and (min-width: 1200px) {
    .landing {
      width: var(--width-desktop);
    }
  }

   /* @media screen and (max-height: 760px) {
     .landing {
       height: 100%;
     }
   } */
</style>
