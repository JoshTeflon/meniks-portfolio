<script>
import LogoEmiSvg from "./icons/LogoEmiSvg.vue";
	export default {
    name: "Footer",
    components: { LogoEmiSvg }
}
</script>

<template>
  <footer class="footer">
    <div class="footer-wrapper">
        <div class="footer-section--1">
            <div class="footer-logo">
                <LogoEmiSvg />
            </div>
            <div>
                <a href=""></a>
                <a href=""></a>
                <a href=""></a>
            </div>
        </div>
        <ul class="footer-section--2">
            <li>Useful Links</li>
            <li></li>
            <li></li>
            <li></li>
        </ul>
    </div>
    <p>All rights reserved by Meniks 2022</p>
  </footer>
</template>

<style scoped>
  .footer .footer-wrapper .footer-section--1 .footer-logo {
      width: 3rem; 
  }
</style>