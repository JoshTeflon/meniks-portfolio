<script>
	export default {
    name: "HeroImage",
	}
</script>

<template>
  <img class="hero--image" src="../assets/images/heroImage.png" alt="hero image" />
</template>

<style scoped>
  .hero--image {
    width: 23.25rem;
  }

  @media screen and (min-width: 640px) {
    .hero--image {
      width: 24.25rem;
    }
  }
</style>