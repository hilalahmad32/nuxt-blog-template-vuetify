<template>
  <div>
    <NavbarVue />
    <HeroVue />
    <PopularPostVue />
    <LastestPostVue />
    <FooterVue />
  </div>
</template>

<script>
import FooterVue from "../components/front/Footer.vue";
import HeroVue from "../components/front/Hero.vue";
import LastestPostVue from "../components/front/LastestPost.vue";
import NavbarVue from "../components/front/Navbar.vue";
import PopularPostVue from "../components/front/PopularPost.vue";

export default {
  name: "IndexPage",
  head(){
  return{
   title:'Home',
  }
  },
  components: {
    NavbarVue,
    HeroVue,
    PopularPostVue,
    LastestPostVue,
    FooterVue,
  },
};
</script>
